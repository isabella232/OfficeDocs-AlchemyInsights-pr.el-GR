---
title: Κλειδιά αποκατάστασης Bitlocker
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
ms.openlocfilehash: 8708ed76f6abe81582823c8af89db8fffef9a3c5
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505068"
---
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="14326-102">Πρόσβαση σε κλειδιά αποκατάστασης Bitlocker</span><span class="sxs-lookup"><span data-stu-id="14326-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="14326-103">Κατά τη ρύθμιση παραμέτρων της πολιτικής προστασίας τελικού σημείου Bitlocker Intune, είναι δυνατό να καθορίσετε εάν οι πληροφορίες αποκατάστασης Bitlocker θα πρέπει να αποθηκεύονται στο Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="14326-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="14326-104">Εάν αυτή η ρύθμιση έχει ρυθμιστεί, τα αποθηκευμένα δεδομένα αποκατάστασης θα πρέπει να είναι ορατά σε ένα διαχειριστή του Intune ως μέρος της εγγραφής δεδομένων συσκευής στο Intune Devices Blade με δύο τρόπους:</span><span class="sxs-lookup"><span data-stu-id="14326-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="14326-105">Συσκευές - Συσκευές Azure AD -> "Συσκευή" Ή Συσκευές -> Όλες οι συσκευές -> "Συσκευή" -> κλειδιά αποκατάστασης</span><span class="sxs-lookup"><span data-stu-id="14326-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="14326-106">Εναλλακτικά, εάν υπάρχει πρόσβαση διαχειριστή στην ίδια τη συσκευή, μπορείτε να δείτε το κλειδί αποκατάστασης (Password) εκτελώντας την ακόλουθη εντολή από μια αναβαθμισμένη γραμμή εντολών:</span><span class="sxs-lookup"><span data-stu-id="14326-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

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
<span data-ttu-id="14326-107">Εάν η συσκευή ήταν κρυπτογραφημένη πριν από την εγγραφή στο Intune, το κλειδί αποκατάστασης μπορεί να έχει συσχετιστεί με τον "Λογαριασμό Microsoft" (MSA) που χρησιμοποιήθηκε για την είσοδο στη συσκευή κατά τη διαδικασία OOBE.</span><span class="sxs-lookup"><span data-stu-id="14326-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="14326-108">Σε αυτή την περίπτωση, η πρόσβαση και η είσοδος με αυτό το MSA θα πρέπει να  https://onedrive.live.com/recoverykey εμφανίζει τις συσκευές για τις οποίες έχουν αποθηκευτεί τα κλειδιά αποκατάστασης.</span><span class="sxs-lookup"><span data-stu-id="14326-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="14326-109">Εάν η συσκευή κρυπτογραφήθηκε ως αποτέλεσμα της ρύθμισης παραμέτρων μέσω της πολιτικής ομάδας που βασίζεται σε τομέα, οι πληροφορίες αποκατάστασης ενδέχεται να αποθηκευτούν στην υπηρεσία καταλόγου Active Directory εσωτερικής εγκατάστασης.</span><span class="sxs-lookup"><span data-stu-id="14326-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>

<span data-ttu-id="14326-110">Εάν έχετε ρυθμίσει τις παραμέτρους της πολιτικής προστασίας τελικού σημείου για την αποθήκευση του κλειδιού αποκατάστασης στο Azure Active Directory, αλλά δεν έχει γίνει αποστολή του κλειδιού για μια συγκεκριμένη συσκευή, μπορείτε να ενεργοποιήσετε την αποστολή περιστρέφοντας το κλειδί αποκατάστασης για τη συγκεκριμένη συσκευή από την κονσόλα MEM.</span><span class="sxs-lookup"><span data-stu-id="14326-110">If you have configured Endpoint protection policy to store the recovery key in Azure Active Directory but the key for a specific device has not been uploaded, you can trigger the upload by rotating the recovery key for that device from the MEM console.</span></span> <span data-ttu-id="14326-111">Για λεπτομέρειες, ανατρέξτε στο [θέμα Περιστροφή πλήκτρων αποκατάστασης BitLocker.](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys)</span><span class="sxs-lookup"><span data-stu-id="14326-111">For details, see [Rotate BitLocker recovery keys](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).</span></span>

