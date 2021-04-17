---
title: Αντιμετώπιση προβλημάτων με την εγγραφή συσκευών iOS στο Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 14f7a897f0c7504db1b605485e170183c3a1afb2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823463"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="316ea-102">Αντιμετώπιση προβλημάτων με την εγγραφή συσκευών iOS στο Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="316ea-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="316ea-103">Εξετάστε τους πόρους που αναφέρονται παρακάτω για να επιλύσετε το πρόβλημά σας τώρα.</span><span class="sxs-lookup"><span data-stu-id="316ea-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="316ea-104">Ορισμένα συνηθισμένα μηνύματα σφάλματος και βήματα επίλυσης:</span><span class="sxs-lookup"><span data-stu-id="316ea-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="316ea-105">**Το cap της συσκευής έχει φτάσει** Ο χρήστης έχει περισσότερες συσκευές εγγεγραμμένες από το όριο της συσκευής.</span><span class="sxs-lookup"><span data-stu-id="316ea-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="316ea-106">Εξετάστε αυτά τα έγγραφα για να [καταργήσετε μια συσκευή ή](https://docs.microsoft.com/intune/devices-wipe) [να αλλάξετε το όριο της συσκευής.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="316ea-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="316ea-107">**Αυτή η υπηρεσία δεν υποστηρίζεται. Δεν υπάρχει πολιτική εγγραφής: Η** Υπηρεσία ειδοποιήσεων push της Apple (APNS) πρέπει να ρυθμιστεί ή να ανανεωθεί.</span><span class="sxs-lookup"><span data-stu-id="316ea-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="316ea-108">Διαβάστε [αυτό το έγγραφο](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) για οδηγίες σχετικά με τον τρόπο για να το κάνετε αυτό.</span><span class="sxs-lookup"><span data-stu-id="316ea-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="316ea-109">**Ο τύπος άδειας χρήσης δεν είναι έγκυρος ή το όνομα χρήστη δεν αναγνωρίζεται:** Στον χρήστη πρέπει να εκχωρηθεί μια άδεια χρήσης Intune ή EMS.</span><span class="sxs-lookup"><span data-stu-id="316ea-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="316ea-110">Εξετάστε αυτά τα έγγραφα για να εκχωρήσετε μια άδεια χρήσης μέσω: [Του Κέντρου διαχείρισης του Office](https://docs.microsoft.com/intune/licenses-assign) ή της [πύλης Azure.](https://docs.microsoft.com/azure/active-directory/license-users-groups)</span><span class="sxs-lookup"><span data-stu-id="316ea-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="316ea-111">Πρόσθετοι πόροι για την επίλυση του προβλήματος:</span><span class="sxs-lookup"><span data-stu-id="316ea-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="316ea-112">Χρησιμοποιήστε [την Πύλη αντιμετώπισης προβλημάτων intune για](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) να διαγνώσετε και να επιλύσετε συνηθισμένες αποτυχίες εγγραφής.</span><span class="sxs-lookup"><span data-stu-id="316ea-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="316ea-113">Διαβάστε [αυτό το έγγραφο](https://docs.microsoft.com/intune/help-desk-operators) για περισσότερες λεπτομέρειες.</span><span class="sxs-lookup"><span data-stu-id="316ea-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="316ea-114">Εξετάστε αυτά τα έγγραφα για μια λίστα με συνήθη σφάλματα που εμποδίζουν την εγγραφή και τις λύσεις σε καθένα: [Οδηγός αντιμετώπισης προβλημάτων και](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) [έγγραφο αντιμετώπισης προβλημάτων.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="316ea-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="316ea-115">[Μάθετε πώς μπορείτε να εγγράψετε συσκευές iOS στο Microsoft Intune.](https://docs.microsoft.com/intune/ios-enroll)</span><span class="sxs-lookup"><span data-stu-id="316ea-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

