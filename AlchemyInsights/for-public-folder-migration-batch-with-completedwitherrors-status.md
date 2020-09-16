---
title: Για τη δέσμη μετεγκατάστασης δημόσιου φακέλου με κατάσταση CompletedWithErrors
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3532"
ms.openlocfilehash: cbf5237fdb5c660057465e67702e35f68e545ddb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744113"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Για τη δέσμη μετεγκατάστασης δημόσιου φακέλου με κατάσταση CompletedWithErrors

Χρησιμοποιήστε τα παρακάτω βήματα για να ολοκληρώσετε τη δέσμη, παρακάμπτοντας τα μεγάλα/κακά στοιχεία: 
1. Έγκριση της δέσμης μεταπήδησης στοιχείων σε μετεγκατάσταση:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Χρησιμοποιήστε την ακόλουθη εντολή για να εγκρίνετε τα στοιχεία που παραλείπονται σε αιτήσεις μετεγκατάστασης που είναι "συγχρονισμένα", αλλά δεν έχουν ολοκληρωθεί:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Η δέσμη μετεγκατάστασης και οι αιτήσεις θα πρέπει να συνεχιστούν και να ολοκληρωθούν σε λίγα λεπτά.

