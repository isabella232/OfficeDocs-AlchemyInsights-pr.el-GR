---
title: Αντιμετώπιση προβλημάτων με την εγγραφή συσκευών Android στο Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 08620a44dcf693482c65ff05e19f11870f67afbe
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830942"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="31e90-102">Αντιμετώπιση προβλημάτων με την εγγραφή συσκευών Android στο Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="31e90-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="31e90-103">Εξετάστε τους πόρους που αναφέρονται παρακάτω για να επιλύσετε το πρόβλημά σας τώρα.</span><span class="sxs-lookup"><span data-stu-id="31e90-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="31e90-104">Ορισμένα συνήθη προβλήματα και βήματα επίλυσης:</span><span class="sxs-lookup"><span data-stu-id="31e90-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="31e90-105">**Σφάλμα "Συσκευή χωρίς κρυπτογράφηση" στην εταιρική πύλη:** Οι νεότερες εκδόσεις του Android, ιδιαίτερα ξεκινώντας από τη v7.0, απαιτούν κωδικό πρόσβασης εκκίνησης για να βεβαιωθούν ότι η συσκευή σας είναι πλήρως κρυπτογραφημένη.</span><span class="sxs-lookup"><span data-stu-id="31e90-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="31e90-106">Οι συνηθισμένες λύσεις είναι να ενεργοποιήσετε μια καρφίτσα εκκίνησης ή να κρυπτογραφήσετε πλήρως τη συσκευή.</span><span class="sxs-lookup"><span data-stu-id="31e90-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="31e90-107">Διαβάστε [αυτό το έγγραφο](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) για περισσότερες πληροφορίες.</span><span class="sxs-lookup"><span data-stu-id="31e90-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="31e90-108">Οι συσκευές δεν μπορούν να μεταδοτούν με την υπηρεσία Intune ή να εμφανίζονται **ως "Ανθυγιεινά" στην κονσόλα διαχείρισης Intune:** Ορισμένες συσκευές Samsung 4.4 και 5.5 ενδέχεται να μην έχουν έλεγχο της υπηρεσίας.</span><span class="sxs-lookup"><span data-stu-id="31e90-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="31e90-109">Υπάρχουν 3 πιθανές λύσεις σε αυτό το πρόβλημα:</span><span class="sxs-lookup"><span data-stu-id="31e90-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="31e90-110">Ανοίξτε με μη αυτόματο τρόπο την εφαρμογή Εταιρική πύλη Intune, η οποία θα ξεκινήσει αυτόματα ένα συγχρονισμό συσκευής.</span><span class="sxs-lookup"><span data-stu-id="31e90-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="31e90-111">Ενημερώστε τη συσκευή σε Android 6.0 ή υψηλότερη έκδοση.</span><span class="sxs-lookup"><span data-stu-id="31e90-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="31e90-112">Απενεργοποιήστε το Samsung Smart Manager από τη διαχείριση της εταιρικής πύλης Intune.</span><span class="sxs-lookup"><span data-stu-id="31e90-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="31e90-113">Διαβάστε [αυτό το έγγραφο](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) για περισσότερες λεπτομέρειες σχετικά με αυτά τα ζητήματα και τις λύσεις.</span><span class="sxs-lookup"><span data-stu-id="31e90-113">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="31e90-114">**Σφάλμα "Μη έγκυρος τύπος** άδειας χρήσης" ή "Μη αναγνωρισμένο όνομα **χρήστη":** Πρέπει να εκχωρηθεί στο χρήστη μια άδεια χρήσης Intune ή EMS.</span><span class="sxs-lookup"><span data-stu-id="31e90-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="31e90-115">Εξετάστε αυτά τα έγγραφα για να εκχωρήσετε μια άδεια χρήσης μέσω: Του Κέντρου διαχείρισης του Office ή της πύλης Azure.</span><span class="sxs-lookup"><span data-stu-id="31e90-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="31e90-116">Πρόσθετοι πόροι για την επίλυση του προβλήματος:</span><span class="sxs-lookup"><span data-stu-id="31e90-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="31e90-117">Χρησιμοποιήστε [την Πύλη αντιμετώπισης προβλημάτων intune για](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) να διαγνώσετε και να επιλύσετε συνηθισμένες αποτυχίες εγγραφής.</span><span class="sxs-lookup"><span data-stu-id="31e90-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="31e90-118">Διαβάστε [αυτό το έγγραφο](https://docs.microsoft.com/intune/help-desk-operators) για περισσότερες λεπτομέρειες.</span><span class="sxs-lookup"><span data-stu-id="31e90-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="31e90-119">Εξετάστε [αυτό το έγγραφο](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) για μια λίστα με συνήθη σφάλματα που εμποδίζουν την εγγραφή και τις λύσεις για το καθένα.</span><span class="sxs-lookup"><span data-stu-id="31e90-119">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="31e90-120">[Μάθετε πώς μπορείτε να εγγράψετε συσκευές Android στο Microsoft Intune.](https://docs.microsoft.com/intune/android-enroll)</span><span class="sxs-lookup"><span data-stu-id="31e90-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
