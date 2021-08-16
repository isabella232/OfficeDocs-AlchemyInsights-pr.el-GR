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
ms.openlocfilehash: 78ceac80626159e72af5f9ac963365c5c057a4ef0de2b3dc7e4cde5e5cc155e5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068164"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Για τη δέσμη μετεγκατάστασης δημόσιου φακέλου με κατάσταση CompletedWithErrors

Ακολουθήστε τα παρακάτω βήματα για να ολοκληρώσετε τη δέσμη, παραλείποντας τα μεγάλα/άσχημα στοιχεία: 
1. Έγκριση των στοιχείων που έχουν παραλειφθεί στη δέσμη μετεγκατάστασης:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Χρησιμοποιήστε την ακόλουθη εντολή για να εγκρίνετε τα στοιχεία που έχουν παραλειφθεί σε αιτήσεις μετεγκατάστασης που έχουν "συγχρονιστεί" αλλά δεν έχουν ολοκληρωθεί:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Η δέσμη μετεγκατάστασης και οι αιτήσεις θα πρέπει να συνεχιστούν και να ολοκληρωθεί σε λίγα λεπτά.

