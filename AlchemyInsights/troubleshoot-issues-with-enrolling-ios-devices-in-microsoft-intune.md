---
title: Αντιμετώπιση προβλημάτων με την εγγραφή συσκευών iOS στο Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: bdbfe7bae00a4c5cfa0edbe9a37522cc98e52401
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 10/18/2019
ms.locfileid: "36506965"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Αντιμετώπιση προβλημάτων με την εγγραφή συσκευών iOS στο Microsoft Intune

Εξετάστε τους πόρους που αναφέρονται παρακάτω για να επιλύσετε το πρόβλημά σας τώρα. 
  
Ορισμένα συνηθισμένα μηνύματα σφάλματος και βήματα επίλυσης:
  
- **Έφτασε το καπάκι της συσκευής** Ο χρήστης έχει περισσότερες συσκευές εγγεγραμμένοι από το όριο της συσκευής. Εξετάστε αυτά τα έγγραφα για να [καταργήσετε μια συσκευή](https://docs.microsoft.com/intune/devices-wipe) ή να [αλλάξετε το όριο της συσκευής](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Αυτή η υπηρεσία δεν υποστηρίζεται. Δεν υπάρχει πολιτική εγγραφής:** η υπηρεσία ειδοποιήσεων push της Apple (APNS) πρέπει να ρυθμιστεί ή να ανανεωθεί. Εξετάστε [αυτό το έγγραφο](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) για οδηγίες σχετικά με το πώς να το κάνετε αυτό. 
    
- **Τύπος άδειας χρήσης δεν είναι έγκυρος ή το όνομα χρήστη δεν αναγνωρίζεται:** Ο χρήστης πρέπει να εκχωρηθεί μια άδεια Intune ή EMS. Εξετάστε αυτά τα έγγραφα για να αντιστοιχίσετε μια άδεια χρήσης μέσω: [Κέντρο διαχείρισης του Office](https://docs.microsoft.com/intune/licenses-assign) ή [Azure πύλης](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Πρόσθετοι πόροι που θα σας βοηθήσουν να επιλύσετε το πρόβλημά σας:
  
1. Χρησιμοποιήστε την [πύλη αντιμετώπισης προβλημάτων Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) για να διαγνώσετε και να επιλύσετε συνηθισμένες αποτυχίες εγγραφής. Εξετάστε [αυτό το έγγραφο](https://docs.microsoft.com/intune/help-desk-operators) για περισσότερες λεπτομέρειες. 
    
2. Εξετάστε αυτά τα έγγραφα για μια λίστα συνηθισμένων σφαλμάτων που εμποδίζουν την εγγραφή και τις αναλύσεις σε κάθε μία: [Οδηγός αντιμετώπισης προβλημάτων](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) και [Αντιμετώπιση προβλημάτων doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Μάθετε πώς μπορείτε να εγγράψετε συσκευές iOS στο Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

