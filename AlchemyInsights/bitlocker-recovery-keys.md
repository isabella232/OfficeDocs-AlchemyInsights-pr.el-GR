---
title: Κλειδιά αποκατάστασης BitLocker
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
- "1922"
- "9000220"
ms.openlocfilehash: 7c56e68cf303939d8e7d4ee0a7301e367ecfe9f9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685886"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Πρόσβαση σε κλειδιά αποκατάστασης BitLocker

Κατά τη ρύθμιση των παραμέτρων της πολιτικής προστασίας απόληξης των ρυθμίσεων BitLocker, είναι δυνατό να καθορίσετε εάν οι πληροφορίες αποκατάστασης BitLocker πρέπει να αποθηκεύονται στο Azure Active Directory.

Εάν αυτή η ρύθμιση έχει ρυθμιστεί, τα αποθηκευμένα δεδομένα αποκατάστασης θα πρέπει να είναι ορατά σε ένα διαχειριστή του Intune ως μέρος της εγγραφής δεδομένων της συσκευής στο Intune Devices blade με δύο τρόπους:

Συσκευές-συσκευές Azure AD-> "συσκευή" ή συσκευές-> όλες οι συσκευές-> "συσκευή"-> κλειδιά αποκατάστασης

Εναλλακτικά, εάν υπάρχει πρόσβαση διαχειριστή στην ίδια τη συσκευή, μπορείτε να δείτε το κλειδί αποκατάστασης (κωδικός πρόσβασης) εκτελώντας την ακόλουθη εντολή από μια γραμμή εντολών με αυξημένα δικαιώματα:

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
Εάν η συσκευή ήταν κρυπτογραφημένη πριν από την εγγραφή στο Intune, το κλειδί αποκατάστασης μπορεί να έχει συσχετιστεί με το "λογαριασμό Microsoft" (MSA) που χρησιμοποιείται για την είσοδο στη συσκευή κατά τη διαδικασία OOBE. Σε αυτή την περίπτωση, η πρόσβαση  https://onedrive.live.com/recoverykey και η είσοδος με αυτό το MSA θα πρέπει να εμφανίζει τις συσκευές για τις οποίες έχουν αποθηκευτεί τα κλειδιά αποκατάστασης.
 
Εάν η συσκευή έχει κρυπτογραφηθεί ως αποτέλεσμα της ρύθμισης παραμέτρων μέσω της πολιτικής ομάδας που βασίζεται σε τομέα, οι πληροφορίες αποκατάστασης μπορεί να είναι αποθηκευμένες στην υπηρεσία καταλόγου Active Directory εσωτερικής εγκατάστασης.
 

