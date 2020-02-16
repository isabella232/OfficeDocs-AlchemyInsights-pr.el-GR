---
title: Για τη δέσμη μετεγκατάστασης δημόσιου φακέλου με κατάσταση CompletedWithErrors
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3532"
ms.openlocfilehash: 4243cdf0170fed1eadac6560d2a04e1a861c63e5
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 02/15/2020
ms.locfileid: "42043589"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a><span data-ttu-id="c18bd-102">Για τη δέσμη μετεγκατάστασης δημόσιου φακέλου με κατάσταση CompletedWithErrors</span><span class="sxs-lookup"><span data-stu-id="c18bd-102">For Public folder migration batch with CompletedWithErrors status</span></span>

<span data-ttu-id="c18bd-103">Χρησιμοποιήστε τα ακόλουθα βήματα για να ολοκληρώσετε τη δέσμη, παρακάμπτοντας τα μεγάλα/κακά στοιχεία:</span><span class="sxs-lookup"><span data-stu-id="c18bd-103">Use the following steps to complete the batch, skipping the large/bad items:</span></span> 
1. <span data-ttu-id="c18bd-104">Έγκριση των στοιχείων που παραλείπονται στη δέσμη μετεγκατάστασης:</span><span class="sxs-lookup"><span data-stu-id="c18bd-104">Approve the skipped items on migration batch:</span></span>

    <span data-ttu-id="c18bd-105">Set-MigrationBatch \<batchname>-ApproveSkippedItems</span><span class="sxs-lookup"><span data-stu-id="c18bd-105">Set-MigrationBatch \<batchname> -ApproveSkippedItems</span></span> 
2. <span data-ttu-id="c18bd-106">Χρησιμοποιήστε την ακόλουθη εντολή για να εγκρίνετε τα στοιχεία που παραλείπονται σε αιτήσεις μετεγκατάστασης που είναι "συγχρονισμένες" αλλά δεν έχουν ολοκληρωθεί:</span><span class="sxs-lookup"><span data-stu-id="c18bd-106">Use the following command to approve the skipped items on migration requests that are “Synced” but not completed:</span></span>

    <span data-ttu-id="c18bd-107">$pf = Πάρτε-PublicFolderMailboxMigrationRequest | Πάρτε-PublicFolderMailboxMigrationRequestStatistics-IncludeReport? ForEach ($i σε $pf) {IF ($i. LargeItemsEncountered-gt 0-ή $i. BadItemsEncountered-gt 0) {Set-PublicFolderMailboxMigrationRequest $i. Identity. IdentifyingGuid-SkippedItemApprovalTime $ ([ημερομηνία ημερομηνίας]:: UtcNow)}}</span><span class="sxs-lookup"><span data-stu-id="c18bd-107">$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}</span></span>
3. <span data-ttu-id="c18bd-108">Η παρτίδα μετεγκατάστασης και οι αιτήσεις θα πρέπει να συνεχιστούν και να ολοκληρωθούν σε λίγα λεπτά.</span><span class="sxs-lookup"><span data-stu-id="c18bd-108">The migration batch and requests should resume and complete in a few minutes.</span></span>

