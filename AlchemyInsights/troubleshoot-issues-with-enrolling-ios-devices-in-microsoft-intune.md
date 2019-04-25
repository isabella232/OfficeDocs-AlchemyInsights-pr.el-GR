---
title: Αντιμετώπιση προβλημάτων σχετικά με την εγγραφή συσκευών iOS στο Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: d28dca4fccf823e627dd179f828ba3b8baf843a6
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32391007"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="acf9b-102">Αντιμετώπιση προβλημάτων σχετικά με την εγγραφή συσκευών iOS στο Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="acf9b-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="acf9b-103">Εξετάστε τους πόρους που αναφέρονται παρακάτω για να επιλύσετε το θέμα σας τώρα.</span><span class="sxs-lookup"><span data-stu-id="acf9b-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="acf9b-104">Ορισμένα κοινά μηνύματα λάθους και τα βήματα επίλυσης:</span><span class="sxs-lookup"><span data-stu-id="acf9b-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="acf9b-105">**Συσκευή καπέλο φτάσει** Ο χρήστης έχει περισσότερες συσκευές που συμμετέχουν από το όριο συσκευής.</span><span class="sxs-lookup"><span data-stu-id="acf9b-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="acf9b-106">Εξετάστε αυτά τα έγγραφα για να [καταργήσετε μια συσκευή](https://docs.microsoft.com/intune/devices-wipe) ή να [αλλάξετε το όριο της συσκευής](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="acf9b-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="acf9b-107">**Η υπηρεσία αυτή δεν υποστηρίζεται. Δεν υπάρχει πολιτική εγγραφής:** Apple Ώθηση ειδοποίησης υπηρεσίας (APN, τα) πρέπει να ρυθμιστεί ή να ανανεωθεί.</span><span class="sxs-lookup"><span data-stu-id="acf9b-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="acf9b-108">Αναθεωρήστε [αυτό το έγγραφο](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) για οδηγίες σχετικά με τον τρόπο για να το κάνετε.</span><span class="sxs-lookup"><span data-stu-id="acf9b-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="acf9b-109">**Τύπος άδειας χρήστη δεν είναι έγκυρος ή δεν αναγνωρίζεται το όνομα χρήστη:** Ο χρήστης πρέπει να εκχωρηθεί άδεια χρήσης Intune ή EMS.</span><span class="sxs-lookup"><span data-stu-id="acf9b-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="acf9b-110">Εξετάστε αυτά τα έγγραφα για να αναθέσετε μια άδεια χρήσης μέσω: [Κέντρο διαχείρισης του Office](https://docs.microsoft.com/intune/licenses-assign) ή [Azure πύλης](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="acf9b-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="acf9b-111">Πρόσθετους πόρους για να σας βοηθήσουν να επιλύσετε το ζήτημα:</span><span class="sxs-lookup"><span data-stu-id="acf9b-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="acf9b-112">Χρησιμοποιήστε [Πύλη του Intune αντιμετώπιση προβλημάτων](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) για να διαγνώσετε και να επιλύσετε συνηθισμένα σφάλματα εγγραφής.</span><span class="sxs-lookup"><span data-stu-id="acf9b-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="acf9b-113">Αναθεωρήστε [αυτό το έγγραφο](https://docs.microsoft.com/intune/help-desk-operators) για περισσότερες λεπτομέρειες.</span><span class="sxs-lookup"><span data-stu-id="acf9b-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="acf9b-114">Εξετάστε αυτά τα έγγραφα για μια λίστα με συνηθισμένα σφάλματα που εμποδίζουν την εγγραφή και λύσεις σε κάθε: [Οδηγός αντιμετώπισης προβλημάτων](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) και [Αντιμετώπιση προβλημάτων doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="acf9b-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="acf9b-115">[Μάθετε πώς να εγγραφεί iOS συσκευές στη Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="acf9b-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

