---
title: Αντιμετώπιση προβλημάτων με την εγγραφή συσκευών Android στο Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: cc8c68a1e838f67c4510002b2c7ff5294a4649fe
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708998"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="a5cb8-102">Αντιμετώπιση προβλημάτων με την εγγραφή συσκευών Android στο Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="a5cb8-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="a5cb8-103">Εξετάστε τους πόρους που παρατίθενται παρακάτω για να επιλύσετε το πρόβλημά σας τώρα.</span><span class="sxs-lookup"><span data-stu-id="a5cb8-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="a5cb8-104">Ορισμένα συνήθη προβλήματα και βήματα επίλυσης:</span><span class="sxs-lookup"><span data-stu-id="a5cb8-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="a5cb8-105">**Σφάλμα "Η συσκευή δεν είναι κρυπτογραφημένο" στην εταιρική πύλη:** Για τις νεότερες εκδόσεις του Android, ιδιαίτερα όταν ξεκινούν με v7.0, απαιτείται κωδικός πρόσβασης εκκίνησης για να βεβαιωθείτε ότι η συσκευή σας είναι πλήρως κρυπτογραφημένη.</span><span class="sxs-lookup"><span data-stu-id="a5cb8-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="a5cb8-106">Συνήθεις λύσεις είναι να ενεργοποιήσετε μια καρφίτσα εκκίνησης ή να κρυπτογραφήσετε πλήρως τη συσκευή.</span><span class="sxs-lookup"><span data-stu-id="a5cb8-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="a5cb8-107">Διαβάστε [αυτό το έγγραφο](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) για περισσότερες πληροφορίες.</span><span class="sxs-lookup"><span data-stu-id="a5cb8-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="a5cb8-108">Ο έλεγχος της υπηρεσίας Intune στις συσκευές αποτυγχάνουν ή εμφανίζεται ως **"Μη εύρυθμη λειτουργία" στην κονσόλα διαχείρισης του Intune:** Ορισμένες συσκευές Samsung 4.4 και 5.5 ενδέχεται να μην check into the service.</span><span class="sxs-lookup"><span data-stu-id="a5cb8-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="a5cb8-109">Υπάρχουν 3 πιθανές λύσεις σε αυτό το πρόβλημα:</span><span class="sxs-lookup"><span data-stu-id="a5cb8-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="a5cb8-110">Ανοίξτε με μη αυτόματο τρόπο την εφαρμογή Εταιρική πύλη του Intune, η οποία θα ξεκινήσει αυτόματα έναν συγχρονισμό συσκευής.</span><span class="sxs-lookup"><span data-stu-id="a5cb8-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="a5cb8-111">Ενημερώστε τη συσκευή σε Android 6.0 ή υψηλότερη έκδοση.</span><span class="sxs-lookup"><span data-stu-id="a5cb8-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="a5cb8-112">Απενεργοποιήστε το Samsung Smart Manager από τη διαχείριση της εταιρικής πύλης Intune.</span><span class="sxs-lookup"><span data-stu-id="a5cb8-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="a5cb8-113">Διαβάστε [αυτό το έγγραφο](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) για περισσότερες λεπτομέρειες σχετικά με αυτά τα ζητήματα και τις λύσεις.</span><span class="sxs-lookup"><span data-stu-id="a5cb8-113">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="a5cb8-114">**Σφάλμα "Μη έγκυρος τύπος** **άδειας χρήσης"** ή "Δεν αναγνωρίζεται το όνομα χρήστη": Στο χρήστη πρέπει να εκχωρηθεί μια άδεια χρήσης Intune ή EMS.</span><span class="sxs-lookup"><span data-stu-id="a5cb8-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="a5cb8-115">Εξετάστε αυτά τα έγγραφα για να εκχωρήσετε μια άδεια χρήσης μέσω: Κέντρο διαχείρισης του Office ή πύλη Azure.</span><span class="sxs-lookup"><span data-stu-id="a5cb8-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="a5cb8-116">Πρόσθετοι πόροι που θα σας βοηθήσουν να επιλύσετε το πρόβλημα:</span><span class="sxs-lookup"><span data-stu-id="a5cb8-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="a5cb8-117">Χρησιμοποιήστε [την Πύλη αντιμετώπισης προβλημάτων του Intune για](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) τη διάγνωση και την επίλυση συνηθισμένων αποτυχιών εγγραφής.</span><span class="sxs-lookup"><span data-stu-id="a5cb8-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="a5cb8-118">Διαβάστε [αυτό το έγγραφο](https://docs.microsoft.com/intune/help-desk-operators) για περισσότερες λεπτομέρειες.</span><span class="sxs-lookup"><span data-stu-id="a5cb8-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="a5cb8-119">Εξετάστε [αυτό το έγγραφο](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) για μια λίστα με συνηθισμένα σφάλματα που εμποδίζουν την εγγραφή και την επίλυση του καθένα.</span><span class="sxs-lookup"><span data-stu-id="a5cb8-119">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="a5cb8-120">[Μάθετε πώς μπορείτε να εγγράψετε συσκευές Android στο Microsoft Intune.](https://docs.microsoft.com/intune/android-enroll)</span><span class="sxs-lookup"><span data-stu-id="a5cb8-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
