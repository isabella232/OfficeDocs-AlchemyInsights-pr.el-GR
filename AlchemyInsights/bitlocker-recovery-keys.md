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
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="045ff-102">Πρόσβαση σε κλειδιά αποκατάστασης BitLocker</span><span class="sxs-lookup"><span data-stu-id="045ff-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="045ff-103">Κατά τη ρύθμιση παραμέτρων του BitLocker ρυθμίσεις Intune Endpoint προστασίας, είναι δυνατό να καθορίσετε εάν οι πληροφορίες αποκατάστασης BitLocker θα πρέπει να αποθηκεύονται στο Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="045ff-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="045ff-104">Εάν αυτή η ρύθμιση έχει ρυθμιστεί, τα αποθηκευμένα δεδομένα ανάκτησης θα πρέπει να είναι ορατά σε έναν διαχειριστή Intune ως μέρος των δεδομένων καρτέλας της συσκευής στο Intune συσκευές blade με δύο τρόπους:</span><span class="sxs-lookup"><span data-stu-id="045ff-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="045ff-105">Συσκευές-συσκευές AD Azure-> "συσκευή" ή συσκευές-> όλες οι συσκευές-> "συσκευή"-> κλειδιά ανάκτησης</span><span class="sxs-lookup"><span data-stu-id="045ff-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="045ff-106">Εναλλακτικά, εάν υπάρχει πρόσβαση διαχειριστή στην ίδια τη συσκευή, το κλειδί αποκατάστασης (κωδικός πρόσβασης) μπορεί να παρατηρηθεί, εκτελώντας την ακόλουθη εντολή από μια γραμμή εντολών με αυξημένα δικαιώματα:</span><span class="sxs-lookup"><span data-stu-id="045ff-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

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
<span data-ttu-id="045ff-107">Εάν η συσκευή κρυπτογραφήθηκε πριν από την εγγραφή στο Intune, το κλειδί αποκατάστασης μπορεί να έχει συσχετιστεί με το "λογαριασμός Microsoft" (MSA) που χρησιμοποιείται για να εισέλθετε στη συσκευή κατά τη διαδικασία OOBE.</span><span class="sxs-lookup"><span data-stu-id="045ff-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="045ff-108">Σε αυτήν την περίπτωση, η πρόσβαση https://onedrive.live.com/recoverykey και η σύνδεση με αυτό το MSA θα πρέπει να εμφανίζουν τις συσκευές για τις οποίες αποθηκεύτηκαν τα κλειδιά ανάκτησης.</span><span class="sxs-lookup"><span data-stu-id="045ff-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="045ff-109">Εάν η συσκευή κρυπτογραφήθηκε ως αποτέλεσμα της ρύθμισης παραμέτρων μέσω πολιτικής ομάδας που βασίζεται σε τομέα, οι πληροφορίες ανάκτησης ενδέχεται να αποθηκευτούν στην υπηρεσία Active Directory εσωτερικής εγκατάστασης.</span><span class="sxs-lookup"><span data-stu-id="045ff-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>
 

