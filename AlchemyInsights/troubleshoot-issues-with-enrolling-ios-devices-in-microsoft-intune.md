---
title: Αντιμετώπιση προβλημάτων σχετικά με την εγγραφή συσκευών iOS στο Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: cd1afc83fe98f363aee4c3324a634c200cd08947
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29658439"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="0d0c6-102">Αντιμετώπιση προβλημάτων σχετικά με την εγγραφή συσκευών iOS στο Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="0d0c6-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="0d0c6-103">Εξετάστε τους πόρους που αναφέρονται παρακάτω για να επιλύσετε το θέμα σας τώρα.</span><span class="sxs-lookup"><span data-stu-id="0d0c6-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="0d0c6-104">Ορισμένα κοινά μηνύματα λάθους και τα βήματα επίλυσης:</span><span class="sxs-lookup"><span data-stu-id="0d0c6-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="0d0c6-p101">**Συσκευή καπέλο φτάσει** Ο χρήστης έχει περισσότερες συσκευές που συμμετέχουν από το όριο συσκευής. Εξετάστε αυτά τα έγγραφα για να [καταργήσετε μια συσκευή](https://docs.microsoft.com/intune/devices-wipe) ή να [αλλάξετε το όριο της συσκευής](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="0d0c6-p101">**Device Cap Reached** The user has more devices enrolled than the device limit. Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="0d0c6-p102">**Η υπηρεσία αυτή δεν υποστηρίζεται. Δεν υπάρχει πολιτική εγγραφής:** Apple Ώθηση ειδοποίησης υπηρεσίας (APN, τα) πρέπει να ρυθμιστεί ή να ανανεωθεί. Αναθεωρήστε [αυτό το έγγραφο](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) για οδηγίες σχετικά με τον τρόπο για να το κάνετε.</span><span class="sxs-lookup"><span data-stu-id="0d0c6-p102">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed. Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="0d0c6-p103">**Τύπος άδειας χρήστη δεν είναι έγκυρος ή δεν αναγνωρίζεται το όνομα χρήστη:** Ο χρήστης πρέπει να εκχωρηθεί άδεια χρήσης Intune ή EMS. Εξετάστε αυτά τα έγγραφα για να αναθέσετε μια άδεια χρήσης μέσω: [Κέντρο διαχείρισης του Office](https://docs.microsoft.com/intune/licenses-assign) ή [Azure πύλης](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="0d0c6-p103">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license. Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="0d0c6-111">Πρόσθετους πόρους για να σας βοηθήσουν να επιλύσετε το ζήτημα:</span><span class="sxs-lookup"><span data-stu-id="0d0c6-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="0d0c6-p104">Χρησιμοποιήστε [Πύλη του Intune αντιμετώπιση προβλημάτων](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) για να διαγνώσετε και να επιλύσετε συνηθισμένα σφάλματα εγγραφής. Αναθεωρήστε [αυτό το έγγραφο](https://docs.microsoft.com/intune/help-desk-operators) για περισσότερες λεπτομέρειες.</span><span class="sxs-lookup"><span data-stu-id="0d0c6-p104">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="0d0c6-114">Εξετάστε αυτά τα έγγραφα για μια λίστα με συνηθισμένα σφάλματα που εμποδίζουν την εγγραφή και λύσεις σε κάθε: [Οδηγός αντιμετώπισης προβλημάτων](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) και [Αντιμετώπιση προβλημάτων doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="0d0c6-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="0d0c6-115">[Μάθετε πώς να εγγραφεί iOS συσκευές στη Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="0d0c6-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

