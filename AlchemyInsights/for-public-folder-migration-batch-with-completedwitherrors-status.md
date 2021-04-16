---
title: Για τη δέσμη μετεγκατάστασης δημόσιου φακέλου με κατάσταση CompletedWithErrors
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3532"
ms.openlocfilehash: 9ed21bfb9069b56a4fc59b201bb3ad94c6bb6712
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812464"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Για τη δέσμη μετεγκατάστασης δημόσιου φακέλου με κατάσταση CompletedWithErrors

Ακολουθήστε τα παρακάτω βήματα για να ολοκληρώσετε τη δέσμη, παραλείποντας τα μεγάλα/άσχημα στοιχεία: 
1. Έγκριση των στοιχείων που έχουν παραλειφθεί στη δέσμη μετεγκατάστασης:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Χρησιμοποιήστε την ακόλουθη εντολή για να εγκρίνετε τα στοιχεία που έχουν παραλειφθεί σε αιτήσεις μετεγκατάστασης που έχουν "συγχρονιστεί" αλλά δεν έχουν ολοκληρωθεί:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Η δέσμη μετεγκατάστασης και οι αιτήσεις θα πρέπει να συνεχιστούν και να ολοκληρωθεί σε λίγα λεπτά.

