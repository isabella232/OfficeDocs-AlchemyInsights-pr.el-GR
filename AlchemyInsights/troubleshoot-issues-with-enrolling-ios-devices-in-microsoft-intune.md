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
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Αντιμετώπιση προβλημάτων με την εγγραφή συσκευών iOS στο Microsoft Intune

Εξετάστε τους πόρους που παρατίθενται παρακάτω για να επιλύσετε το πρόβλημά σας τώρα. 
  
Ορισμένα συνήθη μηνύματα σφάλματος και βήματα επίλυσης:
  
- **Όριο συσκευής που έχει επιτευχθεί** Ο χρήστης έχει εγγράψει περισσότερες συσκευές σε σχέση με το όριο συσκευών. Εξετάστε αυτά τα έγγραφα για να [καταργήσετε μια συσκευή ή](https://docs.microsoft.com/intune/devices-wipe) [να αλλάξετε το όριο συσκευών.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)
    
- **Αυτή η υπηρεσία δεν υποστηρίζεται. Καμία πολιτική εγγραφής: Η** υπηρεσία ειδοποιήσεων push της Apple (APNS) πρέπει να ρυθμιστεί ή να ανανεωθεί. Διαβάστε [αυτό το έγγραφο](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) για οδηγίες σχετικά με το πώς να το κάνετε αυτό. 
    
- **Τύπος άδειας χρήσης που δεν είναι έγκυρος ή το όνομα χρήστη δεν αναγνωρίζεται:** Στο χρήστη πρέπει να εκχωρηθεί μια άδεια χρήσης Intune ή EMS. Εξετάστε αυτά τα έγγραφα για να εκχωρήσετε μια άδεια χρήσης μέσω: [Κέντρο διαχείρισης του Office](https://docs.microsoft.com/intune/licenses-assign) ή πύλη [Azure.](https://docs.microsoft.com/azure/active-directory/license-users-groups)
    
Πρόσθετοι πόροι που θα σας βοηθήσουν να επιλύσετε το πρόβλημα:
  
1. Χρησιμοποιήστε [την Πύλη αντιμετώπισης προβλημάτων του Intune για](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) τη διάγνωση και την επίλυση συνηθισμένων αποτυχιών εγγραφής. Διαβάστε [αυτό το έγγραφο](https://docs.microsoft.com/intune/help-desk-operators) για περισσότερες λεπτομέρειες. 
    
2. Εξετάστε αυτά τα έγγραφα για μια λίστα με συνηθισμένα σφάλματα που εμποδίζουν την εγγραφή και την επίλυση του [καθένα:](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) Οδηγός αντιμετώπισης προβλημάτων και [έγγραφο αντιμετώπισης προβλημάτων.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)
    
3. [Μάθετε πώς μπορείτε να εγγράψετε συσκευές iOS στο Microsoft Intune.](https://docs.microsoft.com/intune/ios-enroll)
    

