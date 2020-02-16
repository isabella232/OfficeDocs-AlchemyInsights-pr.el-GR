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
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Για τη δέσμη μετεγκατάστασης δημόσιου φακέλου με κατάσταση CompletedWithErrors

Χρησιμοποιήστε τα ακόλουθα βήματα για να ολοκληρώσετε τη δέσμη, παρακάμπτοντας τα μεγάλα/κακά στοιχεία: 
1. Έγκριση των στοιχείων που παραλείπονται στη δέσμη μετεγκατάστασης:

    Set-MigrationBatch \<batchname>-ApproveSkippedItems 
2. Χρησιμοποιήστε την ακόλουθη εντολή για να εγκρίνετε τα στοιχεία που παραλείπονται σε αιτήσεις μετεγκατάστασης που είναι "συγχρονισμένες" αλλά δεν έχουν ολοκληρωθεί:

    $pf = Πάρτε-PublicFolderMailboxMigrationRequest | Πάρτε-PublicFolderMailboxMigrationRequestStatistics-IncludeReport? ForEach ($i σε $pf) {IF ($i. LargeItemsEncountered-gt 0-ή $i. BadItemsEncountered-gt 0) {Set-PublicFolderMailboxMigrationRequest $i. Identity. IdentifyingGuid-SkippedItemApprovalTime $ ([ημερομηνία ημερομηνίας]:: UtcNow)}}
3. Η παρτίδα μετεγκατάστασης και οι αιτήσεις θα πρέπει να συνεχιστούν και να ολοκληρωθούν σε λίγα λεπτά.

