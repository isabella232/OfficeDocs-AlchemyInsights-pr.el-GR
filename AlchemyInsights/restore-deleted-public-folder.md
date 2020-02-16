---
title: Επαναφορά ενός διαγραμμένου δημόσιου φακέλου
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
- "3488"
ms.openlocfilehash: 7b04612daca61650d162c1dde240e25c1b185b04
ms.sourcegitcommit: 8ba12eff67e405f5922ea4cc35155e3036447859
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 02/15/2020
ms.locfileid: "42063658"
---
# <a name="restore-a-deleted-public-folder"></a>Επαναφορά ενός διαγραμμένου δημόσιου φακέλου

**Για να επαναφέρετε τα διαγραμμένα στοιχεία από έναν δημόσιο φάκελο**:

- Δείτε [δεν μπορείτε να ανακτήσετε διαγραμμένα στοιχεία από ένα δημόσιο φάκελο μη αλληλογραφίας στο Outlook 2016](https://aka.ms/pfrec).
 
**Για να επαναφέρετε ένα διαγραμμένο δημόσιο φάκελο (οποιουδήποτε τύπου)**: 

- Παρακαλώ χρησιμοποιήστε μετά έξω PowerShell εντολή:

    Σύνταξη:

    >$pf = Πάρτε-PublicFolder \ NON_IPM_SUBTREE \ DUMPSTER_ROOT-αναραστεί |; {$_. Όνομα-EQ "\<name_of_deleted_public_Folder"}; Set-PublicFolder $pf. διαδρομή ταυτότητας- \<διαδρομής όπου θα αποκατασταθεί ο φάκελος>

    Παράδειγμα: η ακόλουθη εντολή θα αποκαταστήσει το Subfolder1 και θα το τοποθετήσει κάτω από \Parent1:

    >$pf = Πάρτε-PublicFolder \ NON_IPM_SUBTREE \ DUMPSTER_ROOT-αναραστεί |; {$_. Όνομα-EQ "Subfolder1"}; Set-PublicFolder $pf. ταυτότητα-διαδρομή \Parent1

Ανατρέξτε [στο φάκελο επαναφορά ενός διαγραμμένου δημόσιου φακέλου](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) για περισσότερες λεπτομέρειες.
