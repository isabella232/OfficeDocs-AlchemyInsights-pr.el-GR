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
ms.openlocfilehash: 663ff9b101494be781095ca550a4ed3deedca175
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29471525"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Αντιμετώπιση προβλημάτων σχετικά με την εγγραφή συσκευών iOS στο Microsoft Intune

Εξετάστε τους πόρους που αναφέρονται παρακάτω για να επιλύσετε το θέμα σας τώρα. 
  
Ορισμένα κοινά μηνύματα λάθους και τα βήματα επίλυσης:
  
- **Συσκευή καπέλο φτάσει** Ο χρήστης έχει περισσότερες συσκευές που συμμετέχουν από το όριο συσκευής. Εξετάστε αυτά τα έγγραφα για να [καταργήσετε μια συσκευή](https://docs.microsoft.com/en-us/intune/devices-wipe) ή να [αλλάξετε το όριο της συσκευής](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Η υπηρεσία αυτή δεν υποστηρίζεται. Δεν υπάρχει πολιτική εγγραφής:** Apple Ώθηση ειδοποίησης υπηρεσίας (APN, τα) πρέπει να ρυθμιστεί ή να ανανεωθεί. Αναθεωρήστε [αυτό το έγγραφο](https://docs.microsoft.com/en-us/intune/apple-mdm-push-certificate-get) για οδηγίες σχετικά με τον τρόπο για να το κάνετε. 
    
- **Τύπος άδειας χρήστη δεν είναι έγκυρος ή δεν αναγνωρίζεται το όνομα χρήστη:** Ο χρήστης πρέπει να εκχωρηθεί άδεια χρήσης Intune ή EMS. Εξετάστε αυτά τα έγγραφα για να αναθέσετε μια άδεια χρήσης μέσω: [Κέντρο διαχείρισης του Office](https://docs.microsoft.com/en-us/intune/licenses-assign) ή [Azure πύλης](https://docs.microsoft.com/en-us/azure/active-directory/license-users-groups).
    
Πρόσθετους πόρους για να σας βοηθήσουν να επιλύσετε το ζήτημα:
  
1. Χρησιμοποιήστε [Πύλη του Intune αντιμετώπιση προβλημάτων](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) για να διαγνώσετε και να επιλύσετε συνηθισμένα σφάλματα εγγραφής. Αναθεωρήστε [αυτό το έγγραφο](https://docs.microsoft.com/en-us/intune/help-desk-operators) για περισσότερες λεπτομέρειες. 
    
2. Εξετάστε αυτά τα έγγραφα για μια λίστα με συνηθισμένα σφάλματα που εμποδίζουν την εγγραφή και λύσεις σε κάθε: [Οδηγός αντιμετώπισης προβλημάτων](https://support.microsoft.com/en-us/help/4039809/troubleshooting-ios-device-enrollment-in-intune) και [Αντιμετώπιση προβλημάτων doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Μάθετε πώς να εγγραφεί iOS συσκευές στη Microsoft Intune](https://docs.microsoft.com/en-us/intune/ios-enroll).
    

