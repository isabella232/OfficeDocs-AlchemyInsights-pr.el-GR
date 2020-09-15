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
ms.openlocfilehash: b5cb2e8a76e8e7d91bd9cd8789ae1623a7f96579
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47689954"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="d215c-102">Αντιμετώπιση προβλημάτων με την εγγραφή συσκευών Android στο Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="d215c-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="d215c-103">Εξετάστε τους πόρους που παρατίθενται παρακάτω για να επιλύσετε το ζήτημά σας τώρα.</span><span class="sxs-lookup"><span data-stu-id="d215c-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="d215c-104">Ορισμένα συνηθισμένα προβλήματα και βήματα επίλυσης:</span><span class="sxs-lookup"><span data-stu-id="d215c-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="d215c-105">**Σφάλμα συσκευής δεν έχει κρυπτογραφηθεί στην πύλη της εταιρείας:** Οι νεότερες εκδόσεις του Android, κυρίως ξεκινώντας με το v 7.0, απαιτούν έναν κωδικό πρόσβασης εκκίνησης για να βεβαιωθείτε ότι η συσκευή σας είναι πλήρως κρυπτογραφημένη.</span><span class="sxs-lookup"><span data-stu-id="d215c-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="d215c-106">Οι συνήθεις λύσεις είναι να ενεργοποιήσετε ένα PIN εκκίνησης ή να κρυπτογραφήσετε πλήρως τη συσκευή.</span><span class="sxs-lookup"><span data-stu-id="d215c-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="d215c-107">Εξετάστε [αυτό το έγγραφο](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) για περισσότερες πληροφορίες.</span><span class="sxs-lookup"><span data-stu-id="d215c-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="d215c-108">Οι **συσκευές δεν μπορούν να κάνουν μεταβίβαση ελέγχου με την υπηρεσία Intune ή να εμφανίζονται ως "ανθυγιεινά" στην κονσόλα διαχείρισης του Intune:** Ορισμένες συσκευές Samsung 4,4 και 5,5 ενδέχεται να μην ελέγχουν την υπηρεσία.</span><span class="sxs-lookup"><span data-stu-id="d215c-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="d215c-109">Υπάρχουν 3 πιθανές λύσεις για αυτό το πρόβλημα:</span><span class="sxs-lookup"><span data-stu-id="d215c-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="d215c-110">Ανοίξτε με μη αυτόματο τρόπο την εφαρμογή εταιρεία πύλης Intune, η οποία θα ξεκινήσει αυτόματα ένα συγχρονισμό συσκευής.</span><span class="sxs-lookup"><span data-stu-id="d215c-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="d215c-111">Ενημερώστε τη συσκευή σε Android 6,0 ή νεότερη έκδοση.</span><span class="sxs-lookup"><span data-stu-id="d215c-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="d215c-112">Απενεργοποιήστε το Samsung Smart Manager από τη διαχείριση της πύλης της εταιρείας Intune.</span><span class="sxs-lookup"><span data-stu-id="d215c-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="d215c-113">Εξετάστε [αυτό το έγγραφο](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) για περισσότερες λεπτομέρειες σχετικά με αυτά τα θέματα και τις αναλύσεις.</span><span class="sxs-lookup"><span data-stu-id="d215c-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="d215c-114">Ο **τύπος άδειας χρήσης χρήστη δεν είναι έγκυρος** ή το **όνομα χρήστη δεν αναγνωρίζεται ως σφάλμα:** ο χρήστης πρέπει να αντιστοιχιστεί σε μια άδεια χρήσης Intune ή EMS.</span><span class="sxs-lookup"><span data-stu-id="d215c-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="d215c-115">Εξετάστε αυτά τα έγγραφα για να εκχωρήσετε μια άδεια χρήσης μέσω: Κέντρο διαχείρισης του Office ή πύλη Azure.</span><span class="sxs-lookup"><span data-stu-id="d215c-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="d215c-116">Πρόσθετοι πόροι που θα σας βοηθήσουν να επιλύσετε το πρόβλημα:</span><span class="sxs-lookup"><span data-stu-id="d215c-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="d215c-117">Χρησιμοποιήστε την [πύλη αντιμετώπισης προβλημάτων του Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) για να διαγνώσετε και να επιλύσετε συνηθισμένες αποτυχίες εγγραφής.</span><span class="sxs-lookup"><span data-stu-id="d215c-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="d215c-118">Εξετάστε [αυτό το έγγραφο](https://docs.microsoft.com/intune/help-desk-operators) για περισσότερες λεπτομέρειες.</span><span class="sxs-lookup"><span data-stu-id="d215c-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="d215c-119">Εξετάστε [αυτό το έγγραφο](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) για μια λίστα με συνηθισμένα σφάλματα που εμποδίζουν την εγγραφή και τις αναλύσεις σε κάθε μία από αυτές.</span><span class="sxs-lookup"><span data-stu-id="d215c-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="d215c-120">[Μάθετε πώς μπορείτε να εγγράψετε συσκευές Android στο Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="d215c-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
