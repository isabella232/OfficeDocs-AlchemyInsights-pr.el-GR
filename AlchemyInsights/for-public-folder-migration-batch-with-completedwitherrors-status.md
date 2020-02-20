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
ms.openlocfilehash: 739e9d91f90e4c0374814d199e4372eb5625553a
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158606"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Για τη δέσμη μετεγκατάστασης δημόσιου φακέλου με κατάσταση CompletedWithErrors

Χρησιμοποιήστε τα ακόλουθα βήματα για να ολοκληρώσετε τη δέσμη, παρακάμπτοντας τα μεγάλα/κακά στοιχεία: 
1. Έγκριση των στοιχείων που παραλείπονται στη δέσμη μετεγκατάστασης:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Χρησιμοποιήστε την ακόλουθη εντολή για να εγκρίνετε τα στοιχεία που παραλείπονται σε αιτήσεις μετεγκατάστασης που είναι "συγχρονισμένες" αλλά δεν έχουν ολοκληρωθεί:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Η παρτίδα μετεγκατάστασης και οι αιτήσεις θα πρέπει να συνεχιστούν και να ολοκληρωθούν σε λίγα λεπτά.

