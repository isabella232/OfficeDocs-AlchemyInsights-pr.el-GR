---
title: Αντιμετώπιση προβλημάτων σχετικά με την εγγραφή Android συσκευές στη Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.openlocfilehash: 2f4fc434128ebe7323f0b8c08aec3be82112bbda
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29471100"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="ced65-102">Αντιμετώπιση προβλημάτων σχετικά με την εγγραφή Android συσκευές στη Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="ced65-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="ced65-103">Εξετάστε τους πόρους που αναφέρονται παρακάτω για να επιλύσετε το θέμα σας τώρα.</span><span class="sxs-lookup"><span data-stu-id="ced65-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="ced65-104">Ορισμένα συνηθισμένα προβλήματα και βήματα επίλυσης:</span><span class="sxs-lookup"><span data-stu-id="ced65-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="ced65-p101">**Συσκευή δεν κρυπτογραφούνται σφάλμα στο εμπόριο εταιρείας:** Νεότερες εκδόσεις του Android, ιδίως από v7.0, απαιτούν έναν κωδικό πρόσβασης εκκίνησης για να βεβαιωθείτε ότι η συσκευή σας είναι πλήρως κρυπτογραφημένη. Συνήθεις λύσεις πρόκειται να ενεργοποιήσετε ένα pin εκκίνησης ή πλήρη κρυπτογράφηση της συσκευής. Αναθεωρήστε [αυτό το έγγραφο](https://docs.microsoft.com/en-us/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) για περισσότερες πληροφορίες.</span><span class="sxs-lookup"><span data-stu-id="ced65-p101">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted. Common solutions are to enable a startup pin or fully encrypt the device. Review [this document](https://docs.microsoft.com/en-us/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span> 
  
 <span data-ttu-id="ced65-p102">**Συσκευές αδυνατούν να ενημερωθείτε από την υπηρεσία Intune ή να εμφανιστεί ως "Unhealthy" στην κονσόλα διαχείρισης του Intune:** Ορισμένα Samsung 4.4 και 5.5 συσκευές δεν μπορούν να ελέγχουν στην υπηρεσία. Υπάρχουν 3 πιθανές λύσεις για αυτό το ζήτημα:</span><span class="sxs-lookup"><span data-stu-id="ced65-p102">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service. There are 3 possible solutions to this issue:</span></span> 
  
1. <span data-ttu-id="ced65-110">Ανοίξτε με μη αυτόματο τρόπο το app Intune εταιρεία πύλη, που θα ξεκινήσει αυτόματα την συσκευή συγχρονισμού.</span><span class="sxs-lookup"><span data-stu-id="ced65-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>
    
2. <span data-ttu-id="ced65-111">Ενημερώστε τη συσκευή με Android 6.0 ή νεότερη έκδοση.</span><span class="sxs-lookup"><span data-stu-id="ced65-111">Update the device to Android 6.0 or higher.</span></span>
    
3. <span data-ttu-id="ced65-p103">Απενεργοποίηση Samsung έξυπνη διαχείριση με τη διαχείριση της πύλης εταιρείας Intune. Εξετάστε [αυτό το έγγραφο](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) για περισσότερες λεπτομέρειες σχετικά με αυτά τα θέματα και λύσεις.</span><span class="sxs-lookup"><span data-stu-id="ced65-p103">Disable Samsung Smart Manager from managing the Intune Company Portal. Review [this document](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span> 
    
 <span data-ttu-id="ced65-p104">**Χρήστης άδεια τύπου δεν είναι έγκυρος** ή **χρήστη όνομα δεν αναγνωρίζεται σφάλμα:** ο χρήστης θα πρέπει να αντιστοιχιστεί μια άδεια Intune ή EMS. Εξετάστε αυτά τα έγγραφα για να αναθέσετε μια άδεια χρήσης μέσω: Κέντρο διαχείρισης του Office ή Azure πύλης.</span><span class="sxs-lookup"><span data-stu-id="ced65-p104">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license. Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span> 
  
<span data-ttu-id="ced65-116">Πρόσθετους πόρους για να σας βοηθήσουν να επιλύσετε το ζήτημα:</span><span class="sxs-lookup"><span data-stu-id="ced65-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="ced65-p105">Χρησιμοποιήστε [Πύλη του Intune αντιμετώπιση προβλημάτων](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) για να διαγνώσετε και να επιλύσετε συνηθισμένα σφάλματα εγγραφής. Αναθεωρήστε [αυτό το έγγραφο](https://docs.microsoft.com/en-us/intune/help-desk-operators) για περισσότερες λεπτομέρειες.</span><span class="sxs-lookup"><span data-stu-id="ced65-p105">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/en-us/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="ced65-119">Αναθεωρήστε [αυτό το έγγραφο](https://docs.microsoft.com/en-us/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) για μια λίστα κοινών σφαλμάτων που εμποδίζουν εγγραφής και λύσεις για κάθε μία.</span><span class="sxs-lookup"><span data-stu-id="ced65-119">Review [this document](https://docs.microsoft.com/en-us/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span> 
    
3. <span data-ttu-id="ced65-120">[Μάθετε πώς μπορείτε να εγγραφείτε Android συσκευές στη Microsoft Intune](https://docs.microsoft.com/en-us/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="ced65-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/en-us/intune/android-enroll).</span></span>
    

