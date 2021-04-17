---
title: Κλειδιά αποκατάστασης Bitlocker
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
- "1922"
- "9000220"
ms.openlocfilehash: ec90e412302c74748e253f2e5430fa4205466f0d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820286"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Πρόσβαση σε κλειδιά αποκατάστασης Bitlocker

Κατά τη ρύθμιση παραμέτρων της πολιτικής προστασίας τελικού σημείου Bitlocker Intune, είναι δυνατό να καθορίσετε εάν οι πληροφορίες αποκατάστασης Bitlocker θα πρέπει να αποθηκεύονται στο Azure Active Directory.

Εάν αυτή η ρύθμιση έχει ρυθμιστεί, τα αποθηκευμένα δεδομένα αποκατάστασης θα πρέπει να είναι ορατά σε ένα διαχειριστή του Intune ως μέρος της εγγραφής δεδομένων συσκευής στο Intune Devices Blade με δύο τρόπους:

Συσκευές - Συσκευές Azure AD -> "Συσκευή" Ή Συσκευές -> Όλες οι συσκευές -> "Συσκευή" -> κλειδιά αποκατάστασης

Εναλλακτικά, εάν υπάρχει πρόσβαση διαχειριστή στην ίδια τη συσκευή, μπορείτε να δείτε το κλειδί αποκατάστασης (Password) εκτελώντας την ακόλουθη εντολή από μια αναβαθμισμένη γραμμή εντολών:

```
manage-bde -protectors c: -get
Example
Volume C: []
All Key Protectors
    TPM:
      ID: {8A5D13D6-7ED9-46C8-A74F-AC3ADF016EC8}
      PCR Validation Profile:
        0, 2, 4, 8, 9, 10, 11
    Numerical Password:
      ID: {DFA26333-XXXX-402C-YYYY-A8C40AF3ZZZZ}
      Password:
        393943-22222-281721-555554-577984-77777-194700-99999
```
Εάν η συσκευή ήταν κρυπτογραφημένη πριν από την εγγραφή στο Intune, το κλειδί αποκατάστασης μπορεί να έχει συσχετιστεί με τον "Λογαριασμό Microsoft" (MSA) που χρησιμοποιήθηκε για την είσοδο στη συσκευή κατά τη διαδικασία OOBE. Σε αυτή την περίπτωση, η πρόσβαση και η είσοδος με αυτό το MSA θα πρέπει να  https://onedrive.live.com/recoverykey εμφανίζει τις συσκευές για τις οποίες έχουν αποθηκευτεί τα κλειδιά αποκατάστασης.
 
Εάν η συσκευή κρυπτογραφήθηκε ως αποτέλεσμα της ρύθμισης παραμέτρων μέσω της πολιτικής ομάδας που βασίζεται σε τομέα, οι πληροφορίες αποκατάστασης ενδέχεται να αποθηκευτούν στην υπηρεσία καταλόγου Active Directory εσωτερικής εγκατάστασης.

Εάν έχετε ρυθμίσει τις παραμέτρους της πολιτικής προστασίας τελικού σημείου για την αποθήκευση του κλειδιού αποκατάστασης στο Azure Active Directory, αλλά δεν έχει γίνει αποστολή του κλειδιού για μια συγκεκριμένη συσκευή, μπορείτε να ενεργοποιήσετε την αποστολή περιστρέφοντας το κλειδί αποκατάστασης για τη συγκεκριμένη συσκευή από την κονσόλα MEM. Για λεπτομέρειες, ανατρέξτε στο [θέμα Περιστροφή πλήκτρων αποκατάστασης BitLocker.](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys)

