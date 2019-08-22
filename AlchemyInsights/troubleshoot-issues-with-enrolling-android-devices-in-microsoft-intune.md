---
title: Αντιμετώπιση προβλημάτων σχετικά με την εγγραφή Android συσκευές στη Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: 1e1d50c31df588a3416d758d40fbd7bde3f73b21
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36500071"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="62096-102">Αντιμετώπιση προβλημάτων σχετικά με την εγγραφή Android συσκευές στη Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="62096-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="62096-103">Εξετάστε τους πόρους που αναφέρονται παρακάτω για να επιλύσετε το θέμα σας τώρα.</span><span class="sxs-lookup"><span data-stu-id="62096-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="62096-104">Ορισμένα συνηθισμένα προβλήματα και βήματα επίλυσης:</span><span class="sxs-lookup"><span data-stu-id="62096-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="62096-105">**Συσκευή δεν κρυπτογραφούνται σφάλμα στο εμπόριο εταιρείας:** Νεότερες εκδόσεις του Android, ιδίως από v7.0, απαιτούν έναν κωδικό πρόσβασης εκκίνησης για να βεβαιωθείτε ότι η συσκευή σας είναι πλήρως κρυπτογραφημένη.</span><span class="sxs-lookup"><span data-stu-id="62096-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="62096-106">Συνήθεις λύσεις πρόκειται να ενεργοποιήσετε ένα pin εκκίνησης ή πλήρη κρυπτογράφηση της συσκευής.</span><span class="sxs-lookup"><span data-stu-id="62096-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="62096-107">Αναθεωρήστε [αυτό το έγγραφο](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) για περισσότερες πληροφορίες.</span><span class="sxs-lookup"><span data-stu-id="62096-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="62096-108">**Συσκευές αδυνατούν να ενημερωθείτε από την υπηρεσία Intune ή να εμφανιστεί ως "Unhealthy" στην κονσόλα διαχείρισης του Intune:** Ορισμένα Samsung 4.4 και 5.5 συσκευές δεν μπορούν να ελέγχουν στην υπηρεσία.</span><span class="sxs-lookup"><span data-stu-id="62096-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="62096-109">Υπάρχουν 3 πιθανές λύσεις για αυτό το ζήτημα:</span><span class="sxs-lookup"><span data-stu-id="62096-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="62096-110">Ανοίξτε με μη αυτόματο τρόπο το app Intune εταιρεία πύλη, που θα ξεκινήσει αυτόματα την συσκευή συγχρονισμού.</span><span class="sxs-lookup"><span data-stu-id="62096-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="62096-111">Ενημερώστε τη συσκευή με Android 6.0 ή νεότερη έκδοση.</span><span class="sxs-lookup"><span data-stu-id="62096-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="62096-112">Απενεργοποίηση Samsung έξυπνη διαχείριση με τη διαχείριση της πύλης εταιρείας Intune.</span><span class="sxs-lookup"><span data-stu-id="62096-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="62096-113">Εξετάστε [αυτό το έγγραφο](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) για περισσότερες λεπτομέρειες σχετικά με αυτά τα θέματα και λύσεις.</span><span class="sxs-lookup"><span data-stu-id="62096-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="62096-114">**Χρήστης άδεια τύπου δεν είναι έγκυρος** ή **χρήστη όνομα δεν αναγνωρίζεται σφάλμα:** ο χρήστης θα πρέπει να αντιστοιχιστεί μια άδεια Intune ή EMS.</span><span class="sxs-lookup"><span data-stu-id="62096-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="62096-115">Εξετάστε αυτά τα έγγραφα για να αναθέσετε μια άδεια χρήσης μέσω: Κέντρο διαχείρισης του Office ή Azure πύλης.</span><span class="sxs-lookup"><span data-stu-id="62096-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="62096-116">Πρόσθετους πόρους για να σας βοηθήσουν να επιλύσετε το ζήτημα:</span><span class="sxs-lookup"><span data-stu-id="62096-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="62096-117">Χρησιμοποιήστε [Πύλη του Intune αντιμετώπιση προβλημάτων](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) για να διαγνώσετε και να επιλύσετε συνηθισμένα σφάλματα εγγραφής.</span><span class="sxs-lookup"><span data-stu-id="62096-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="62096-118">Αναθεωρήστε [αυτό το έγγραφο](https://docs.microsoft.com/intune/help-desk-operators) για περισσότερες λεπτομέρειες.</span><span class="sxs-lookup"><span data-stu-id="62096-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="62096-119">Αναθεωρήστε [αυτό το έγγραφο](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) για μια λίστα κοινών σφαλμάτων που εμποδίζουν εγγραφής και λύσεις για κάθε μία.</span><span class="sxs-lookup"><span data-stu-id="62096-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="62096-120">[Μάθετε πώς μπορείτε να εγγραφείτε Android συσκευές στη Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="62096-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
