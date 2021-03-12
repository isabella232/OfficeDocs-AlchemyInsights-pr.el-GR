---
title: Αντιμετώπιση προβλημάτων με την εγγραφή συσκευών iOS στο Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 4aef78e5921b789b532fecc99380da3274173bdb
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708962"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="c568b-102">Αντιμετώπιση προβλημάτων με την εγγραφή συσκευών iOS στο Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="c568b-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="c568b-103">Εξετάστε τους πόρους που παρατίθενται παρακάτω για να επιλύσετε το πρόβλημά σας τώρα.</span><span class="sxs-lookup"><span data-stu-id="c568b-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="c568b-104">Ορισμένα συνήθη μηνύματα σφάλματος και βήματα επίλυσης:</span><span class="sxs-lookup"><span data-stu-id="c568b-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="c568b-105">**Όριο συσκευής που έχει επιτευχθεί** Ο χρήστης έχει εγγράψει περισσότερες συσκευές σε σχέση με το όριο συσκευών.</span><span class="sxs-lookup"><span data-stu-id="c568b-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="c568b-106">Εξετάστε αυτά τα έγγραφα για να [καταργήσετε μια συσκευή ή](https://docs.microsoft.com/intune/devices-wipe) [να αλλάξετε το όριο συσκευών.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="c568b-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="c568b-107">**Αυτή η υπηρεσία δεν υποστηρίζεται. Καμία πολιτική εγγραφής: Η** υπηρεσία ειδοποιήσεων push της Apple (APNS) πρέπει να ρυθμιστεί ή να ανανεωθεί.</span><span class="sxs-lookup"><span data-stu-id="c568b-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="c568b-108">Διαβάστε [αυτό το έγγραφο](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) για οδηγίες σχετικά με το πώς να το κάνετε αυτό.</span><span class="sxs-lookup"><span data-stu-id="c568b-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="c568b-109">**Τύπος άδειας χρήσης που δεν είναι έγκυρος ή το όνομα χρήστη δεν αναγνωρίζεται:** Στο χρήστη πρέπει να εκχωρηθεί μια άδεια χρήσης Intune ή EMS.</span><span class="sxs-lookup"><span data-stu-id="c568b-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="c568b-110">Εξετάστε αυτά τα έγγραφα για να εκχωρήσετε μια άδεια χρήσης μέσω: [Κέντρο διαχείρισης του Office](https://docs.microsoft.com/intune/licenses-assign) ή πύλη [Azure.](https://docs.microsoft.com/azure/active-directory/license-users-groups)</span><span class="sxs-lookup"><span data-stu-id="c568b-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="c568b-111">Πρόσθετοι πόροι που θα σας βοηθήσουν να επιλύσετε το πρόβλημα:</span><span class="sxs-lookup"><span data-stu-id="c568b-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="c568b-112">Χρησιμοποιήστε [την Πύλη αντιμετώπισης προβλημάτων του Intune για](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) τη διάγνωση και την επίλυση συνηθισμένων αποτυχιών εγγραφής.</span><span class="sxs-lookup"><span data-stu-id="c568b-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="c568b-113">Διαβάστε [αυτό το έγγραφο](https://docs.microsoft.com/intune/help-desk-operators) για περισσότερες λεπτομέρειες.</span><span class="sxs-lookup"><span data-stu-id="c568b-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="c568b-114">Εξετάστε αυτά τα έγγραφα για μια λίστα με συνηθισμένα σφάλματα που εμποδίζουν την εγγραφή και την επίλυση του [καθένα:](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) Οδηγός αντιμετώπισης προβλημάτων και [έγγραφο αντιμετώπισης προβλημάτων.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="c568b-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="c568b-115">[Μάθετε πώς μπορείτε να εγγράψετε συσκευές iOS στο Microsoft Intune.](https://docs.microsoft.com/intune/ios-enroll)</span><span class="sxs-lookup"><span data-stu-id="c568b-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

