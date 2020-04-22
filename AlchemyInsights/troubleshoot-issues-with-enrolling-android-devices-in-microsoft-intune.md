---
title: Αντιμετώπιση προβλημάτων με την εγγραφή συσκευών Android στο Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: bd6d278ebf6cca7fb6e4ac1049deae600b516707
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759620"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="c79fe-102">Αντιμετώπιση προβλημάτων με την εγγραφή συσκευών Android στο Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="c79fe-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="c79fe-103">Εξετάστε τους πόρους που παρατίθενται παρακάτω για να επιλύσετε το ζήτημά σας τώρα.</span><span class="sxs-lookup"><span data-stu-id="c79fe-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="c79fe-104">Ορισμένα συνηθισμένα ζητήματα και βήματα επίλυσης:</span><span class="sxs-lookup"><span data-stu-id="c79fe-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="c79fe-105">**Η συσκευή δεν είναι κρυπτογραφημένο σφάλμα στην εταιρική πύλη:** Οι νεότερες εκδόσεις του Android, ιδιαίτερα ξεκινώντας από το v7.0, απαιτούν έναν κωδικό πρόσβασης εκκίνησης για να βεβαιωθείτε ότι η συσκευή σας είναι πλήρως κρυπτογραφημένη.</span><span class="sxs-lookup"><span data-stu-id="c79fe-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="c79fe-106">Οι συνήθεις λύσεις είναι να ενεργοποιήσετε μια καρφίτσα εκκίνησης ή να κρυπτογραφήσετε πλήρως τη συσκευή.</span><span class="sxs-lookup"><span data-stu-id="c79fe-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="c79fe-107">Εξετάστε [αυτό το έγγραφο](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) για περισσότερες πληροφορίες.</span><span class="sxs-lookup"><span data-stu-id="c79fe-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="c79fe-108">**Οι συσκευές δεν μπορούν να κάνουν μεταβίβαση ελέγχου με την υπηρεσία Intune ή να εμφανίζονται ως "Ανθυγιεινά" στην κονσόλα διαχείρισης Intune:** Ορισμένες συσκευές Samsung 4.4 και 5.5 ενδέχεται να μην κάνουν check-in στην υπηρεσία.</span><span class="sxs-lookup"><span data-stu-id="c79fe-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="c79fe-109">Υπάρχουν 3 πιθανές λύσεις σε αυτό το ζήτημα:</span><span class="sxs-lookup"><span data-stu-id="c79fe-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="c79fe-110">Ανοίξτε με μη αυτόματο τρόπο την εφαρμογή Intune Company Portal, η οποία θα ξεκινήσει αυτόματα ένα συγχρονισμό συσκευών.</span><span class="sxs-lookup"><span data-stu-id="c79fe-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="c79fe-111">Ενημερώστε τη συσκευή σε Android 6.0 ή νεότερη έκδοση.</span><span class="sxs-lookup"><span data-stu-id="c79fe-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="c79fe-112">Απενεργοποιήστε το Samsung Smart Manager από τη διαχείριση της πύλης της εταιρείας Intune.</span><span class="sxs-lookup"><span data-stu-id="c79fe-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="c79fe-113">Εξετάστε [το παρόν έγγραφο](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) για περισσότερες λεπτομέρειες σχετικά με αυτά τα θέματα και τα ψηφίσματα.</span><span class="sxs-lookup"><span data-stu-id="c79fe-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="c79fe-114">**Ο τύπος άδειας χρήσης δεν είναι έγκυρος** ή **το όνομα χρήστη που δεν αναγνωρίζεται σφάλμα:** Ο χρήστης πρέπει να του εκχωρηθεί μια άδεια χρήσης Intune ή EMS.</span><span class="sxs-lookup"><span data-stu-id="c79fe-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="c79fe-115">Εξετάστε αυτά τα έγγραφα για να εκχωρήσετε μια άδεια χρήσης μέσω: Κέντρο διαχείρισης του Office ή πύλη Azure.</span><span class="sxs-lookup"><span data-stu-id="c79fe-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="c79fe-116">Πρόσθετοι πόροι που θα σας βοηθήσουν να επιλύσετε το ζήτημά σας:</span><span class="sxs-lookup"><span data-stu-id="c79fe-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="c79fe-117">Χρησιμοποιήστε την [πύλη αντιμετώπισης προβλημάτων intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) για να διαγνώσετε και να επιλύσετε συνήθεις αποτυχίες εγγραφής.</span><span class="sxs-lookup"><span data-stu-id="c79fe-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="c79fe-118">Εξετάστε [αυτό το έγγραφο](https://docs.microsoft.com/intune/help-desk-operators) για περισσότερες λεπτομέρειες.</span><span class="sxs-lookup"><span data-stu-id="c79fe-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="c79fe-119">Εξετάστε [αυτό το έγγραφο](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) για μια λίστα συνηθισμένων σφαλμάτων που εμποδίζουν την εγγραφή και τις λύσεις σε κάθε έγγραφο.</span><span class="sxs-lookup"><span data-stu-id="c79fe-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="c79fe-120">[Μάθετε πώς μπορείτε να εγγράψετε συσκευές Android στο Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="c79fe-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
