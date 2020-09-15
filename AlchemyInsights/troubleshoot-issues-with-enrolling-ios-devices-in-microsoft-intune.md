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
ms.openlocfilehash: 7d3e0049258a77016250c8a657c8fbcaf8d65212
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47669248"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Αντιμετώπιση προβλημάτων με την εγγραφή συσκευών iOS στο Microsoft Intune

Εξετάστε τους πόρους που παρατίθενται παρακάτω για να επιλύσετε το ζήτημά σας τώρα. 
  
Ορισμένα συνηθισμένα μηνύματα σφάλματος και βήματα επίλυσης:
  
- Το **καπάκι της συσκευής έφτασε** Ο χρήστης έχει περισσότερες συσκευές που έχουν εγγραφεί από το όριο της συσκευής. Εξετάστε αυτά τα έγγραφα για να [καταργήσετε μια συσκευή](https://docs.microsoft.com/intune/devices-wipe) ή να [αλλάξετε το όριο της συσκευής](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Αυτή η υπηρεσία δεν υποστηρίζεται. Δεν υπάρχει πολιτική εγγραφής:** η υπηρεσία ειδοποιήσεων push της Apple (APNS) πρέπει να ρυθμιστεί ή να ανανεωθεί. Εξετάστε [αυτό το έγγραφο](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) για οδηγίες σχετικά με τον τρόπο με τον οποίο μπορείτε να το κάνετε αυτό. 
    
- Ο **τύπος άδειας χρήσης χρήστη δεν είναι έγκυρος ή το όνομα χρήστη δεν αναγνωρίζεται:** Ο χρήστης πρέπει να του εκχωρηθεί μια άδεια χρήσης Intune ή EMS. Εξετάστε αυτά τα έγγραφα για να εκχωρήσετε μια άδεια χρήσης μέσω: [Κέντρο διαχείρισης του Office](https://docs.microsoft.com/intune/licenses-assign) ή [πύλη Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Πρόσθετοι πόροι που θα σας βοηθήσουν να επιλύσετε το πρόβλημα:
  
1. Χρησιμοποιήστε την [πύλη αντιμετώπισης προβλημάτων του Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) για να διαγνώσετε και να επιλύσετε συνηθισμένες αποτυχίες εγγραφής. Εξετάστε [αυτό το έγγραφο](https://docs.microsoft.com/intune/help-desk-operators) για περισσότερες λεπτομέρειες. 
    
2. Εξετάστε αυτά τα έγγραφα για μια λίστα με συνηθισμένα σφάλματα που εμποδίζουν την εγγραφή και τις αναλύσεις σε κάθε: [Οδηγός αντιμετώπισης προβλημάτων](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) και [Αντιμετώπιση προβλημάτων doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Μάθετε πώς μπορείτε να εγγράψετε συσκευές iOS στο Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

