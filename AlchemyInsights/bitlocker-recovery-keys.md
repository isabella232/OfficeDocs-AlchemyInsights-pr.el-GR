---
title: Κλειδιά αποκατάστασης BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 4e06e0e43b63836b9e9cf923e554dd474b82c671
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908815"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Πρόσβαση σε κλειδιά αποκατάστασης BitLocker

Κατά τη ρύθμιση παραμέτρων του BitLocker ρυθμίσεις Intune Endpoint προστασίας, είναι δυνατό να καθορίσετε εάν οι πληροφορίες αποκατάστασης BitLocker θα πρέπει να αποθηκεύονται στο Azure Active Directory.

Εάν αυτή η ρύθμιση έχει ρυθμιστεί, τα αποθηκευμένα δεδομένα ανάκτησης θα πρέπει να είναι ορατά σε έναν διαχειριστή Intune ως μέρος των δεδομένων καρτέλας της συσκευής στο Intune συσκευές blade με δύο τρόπους:

Συσκευές-συσκευές AD Azure-> "συσκευή" ή συσκευές-> όλες οι συσκευές-> "συσκευή"-> κλειδιά ανάκτησης

Εναλλακτικά, εάν υπάρχει πρόσβαση διαχειριστή στην ίδια τη συσκευή, το κλειδί αποκατάστασης (κωδικός πρόσβασης) μπορεί να παρατηρηθεί, εκτελώντας την ακόλουθη εντολή από μια γραμμή εντολών με αυξημένα δικαιώματα:

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
Εάν η συσκευή κρυπτογραφήθηκε πριν από την εγγραφή στο Intune, το κλειδί αποκατάστασης μπορεί να έχει συσχετιστεί με το "λογαριασμός Microsoft" (MSA) που χρησιμοποιείται για να εισέλθετε στη συσκευή κατά τη διαδικασία OOBE. Σε αυτήν την περίπτωση, η πρόσβαση https://onedrive.live.com/recoverykey και η σύνδεση με αυτό το MSA θα πρέπει να εμφανίζουν τις συσκευές για τις οποίες αποθηκεύτηκαν τα κλειδιά ανάκτησης.
 
Εάν η συσκευή κρυπτογραφήθηκε ως αποτέλεσμα της ρύθμισης παραμέτρων μέσω πολιτικής ομάδας που βασίζεται σε τομέα, οι πληροφορίες ανάκτησης ενδέχεται να αποθηκευτούν στην υπηρεσία Active Directory εσωτερικής εγκατάστασης.
 

