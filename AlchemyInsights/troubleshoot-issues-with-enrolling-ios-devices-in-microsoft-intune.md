---
title: Αντιμετώπιση προβλημάτων με την εγγραφή συσκευών iOS στο Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 664c18daca5d8e0ad4a88f41db3ff0dbced606e5
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43736158"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="f610c-102">Αντιμετώπιση προβλημάτων με την εγγραφή συσκευών iOS στο Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="f610c-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="f610c-103">Εξετάστε τους πόρους που παρατίθενται παρακάτω για να επιλύσετε το ζήτημά σας τώρα.</span><span class="sxs-lookup"><span data-stu-id="f610c-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="f610c-104">Ορισμένα συνηθισμένα μηνύματα σφάλματος και βήματα επίλυσης:</span><span class="sxs-lookup"><span data-stu-id="f610c-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="f610c-105">**Επιτεύχθηκε το κάλυμμα της συσκευής** Ο χρήστης έχει περισσότερες συσκευές εγγεγραμμένες από το όριο της συσκευής.</span><span class="sxs-lookup"><span data-stu-id="f610c-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="f610c-106">Εξετάστε αυτά τα έγγραφα για να [καταργήσετε μια συσκευή](https://docs.microsoft.com/intune/devices-wipe) ή [να αλλάξετε το όριο της συσκευής](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="f610c-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="f610c-107">**Αυτή η υπηρεσία δεν υποστηρίζεται. Καμία πολιτική εγγραφής:** Η υπηρεσία ειδοποιήσεων push της Apple (APNS) πρέπει να ρυθμιστεί ή να ανανεωθεί.</span><span class="sxs-lookup"><span data-stu-id="f610c-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="f610c-108">Εξετάστε [αυτό το έγγραφο](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) για οδηγίες σχετικά με τον τρόπο με τον οποίο μπορείτε να το κάνετε αυτό.</span><span class="sxs-lookup"><span data-stu-id="f610c-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="f610c-109">**Ο τύπος άδειας χρήσης δεν είναι έγκυρος ή το όνομα χρήστη δεν αναγνωρίζεται:** Στο χρήστη πρέπει να εκχωρηθεί μια άδεια χρήσης Intune ή EMS.</span><span class="sxs-lookup"><span data-stu-id="f610c-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="f610c-110">Εξετάστε αυτά τα έγγραφα για να εκχωρήσετε μια άδεια χρήσης: [Κέντρο διαχείρισης του Office](https://docs.microsoft.com/intune/licenses-assign) ή πύλη [Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="f610c-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="f610c-111">Πρόσθετοι πόροι που θα σας βοηθήσουν να επιλύσετε το ζήτημά σας:</span><span class="sxs-lookup"><span data-stu-id="f610c-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="f610c-112">Χρησιμοποιήστε την [πύλη αντιμετώπισης προβλημάτων intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) για να διαγνώσετε και να επιλύσετε συνήθεις αποτυχίες εγγραφής.</span><span class="sxs-lookup"><span data-stu-id="f610c-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="f610c-113">Εξετάστε [αυτό το έγγραφο](https://docs.microsoft.com/intune/help-desk-operators) για περισσότερες λεπτομέρειες.</span><span class="sxs-lookup"><span data-stu-id="f610c-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="f610c-114">Εξετάστε αυτά τα έγγραφα για μια λίστα συνηθισμένων σφαλμάτων που εμποδίζουν την εγγραφή και τις λύσεις σε κάθε ένα: [Οδηγός αντιμετώπισης προβλημάτων](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) και [Αντιμετώπιση προβλημάτων εγγράφου](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="f610c-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="f610c-115">[Μάθετε πώς μπορείτε να εγγράψετε συσκευές iOS στο Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="f610c-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

