---
title: Αντιμετώπιση προβλημάτων με την εγγραφή συσκευών iOS σε Microsoft Intune
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
ms.openlocfilehash: 0aaece95effa468af5c906a8bd07e5b00ffa3df37b4e2cb296d64108efec94e9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54047976"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Αντιμετώπιση προβλημάτων με την εγγραφή συσκευών iOS σε Microsoft Intune

Εξετάστε τους πόρους που αναφέρονται παρακάτω για να επιλύσετε το πρόβλημά σας τώρα. 
  
Ορισμένα συνηθισμένα μηνύματα σφάλματος και βήματα επίλυσης:
  
- **Το cap της συσκευής έχει φτάσει** Ο χρήστης έχει περισσότερες συσκευές εγγεγραμμένες από το όριο της συσκευής. Εξετάστε αυτά τα έγγραφα για να [καταργήσετε μια συσκευή ή](https://docs.microsoft.com/intune/devices-wipe) [να αλλάξετε το όριο της συσκευής.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)
    
- **Αυτή η υπηρεσία δεν υποστηρίζεται. Δεν υπάρχει πολιτική εγγραφής: Η** Υπηρεσία ειδοποιήσεων push της Apple (APNS) πρέπει να ρυθμιστεί ή να ανανεωθεί. Διαβάστε [αυτό το έγγραφο](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) για οδηγίες σχετικά με τον τρόπο για να το κάνετε αυτό. 
    
- **Ο τύπος άδειας χρήσης δεν είναι έγκυρος ή το όνομα χρήστη δεν αναγνωρίζεται:** Στον χρήστη πρέπει να εκχωρηθεί μια άδεια χρήσης Intune ή EMS. Εξετάστε αυτά τα έγγραφα για να εκχωρήσετε μια άδεια χρήσης μέσω: [Office Κέντρο διαχείρισης ή](https://docs.microsoft.com/intune/licenses-assign) πύλη [Azure.](https://docs.microsoft.com/azure/active-directory/license-users-groups)
    
Πρόσθετοι πόροι για την επίλυση του προβλήματος:
  
1. Χρησιμοποιήστε [την Πύλη αντιμετώπισης προβλημάτων intune για](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) να διαγνώσετε και να επιλύσετε συνηθισμένες αποτυχίες εγγραφής. Διαβάστε [αυτό το έγγραφο](https://docs.microsoft.com/intune/help-desk-operators) για περισσότερες λεπτομέρειες. 
    
2. Εξετάστε αυτά τα έγγραφα για μια λίστα με συνήθη σφάλματα που εμποδίζουν την εγγραφή και τις λύσεις σε καθένα: [Οδηγός αντιμετώπισης προβλημάτων και](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) [έγγραφο αντιμετώπισης προβλημάτων.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)
    
3. [Μάθετε πώς μπορείτε να εγγράψετε συσκευές iOS στο Microsoft Intune.](https://docs.microsoft.com/intune/ios-enroll)
    

