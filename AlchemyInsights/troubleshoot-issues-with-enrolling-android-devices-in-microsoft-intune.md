---
title: Αντιμετώπιση προβλημάτων με την εγγραφή συσκευών Android στο Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: b5cb2e8a76e8e7d91bd9cd8789ae1623a7f96579
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47689954"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Αντιμετώπιση προβλημάτων με την εγγραφή συσκευών Android στο Microsoft Intune

Εξετάστε τους πόρους που παρατίθενται παρακάτω για να επιλύσετε το ζήτημά σας τώρα.
  
Ορισμένα συνηθισμένα προβλήματα και βήματα επίλυσης:
  
 **Σφάλμα συσκευής δεν έχει κρυπτογραφηθεί στην πύλη της εταιρείας:** Οι νεότερες εκδόσεις του Android, κυρίως ξεκινώντας με το v 7.0, απαιτούν έναν κωδικό πρόσβασης εκκίνησης για να βεβαιωθείτε ότι η συσκευή σας είναι πλήρως κρυπτογραφημένη. Οι συνήθεις λύσεις είναι να ενεργοποιήσετε ένα PIN εκκίνησης ή να κρυπτογραφήσετε πλήρως τη συσκευή. Εξετάστε [αυτό το έγγραφο](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) για περισσότερες πληροφορίες.
  
 Οι **συσκευές δεν μπορούν να κάνουν μεταβίβαση ελέγχου με την υπηρεσία Intune ή να εμφανίζονται ως "ανθυγιεινά" στην κονσόλα διαχείρισης του Intune:** Ορισμένες συσκευές Samsung 4,4 και 5,5 ενδέχεται να μην ελέγχουν την υπηρεσία. Υπάρχουν 3 πιθανές λύσεις για αυτό το πρόβλημα:
  
1. Ανοίξτε με μη αυτόματο τρόπο την εφαρμογή εταιρεία πύλης Intune, η οποία θα ξεκινήσει αυτόματα ένα συγχρονισμό συσκευής.

2. Ενημερώστε τη συσκευή σε Android 6,0 ή νεότερη έκδοση.

3. Απενεργοποιήστε το Samsung Smart Manager από τη διαχείριση της πύλης της εταιρείας Intune. Εξετάστε [αυτό το έγγραφο](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) για περισσότερες λεπτομέρειες σχετικά με αυτά τα θέματα και τις αναλύσεις.

 Ο **τύπος άδειας χρήσης χρήστη δεν είναι έγκυρος** ή το **όνομα χρήστη δεν αναγνωρίζεται ως σφάλμα:** ο χρήστης πρέπει να αντιστοιχιστεί σε μια άδεια χρήσης Intune ή EMS. Εξετάστε αυτά τα έγγραφα για να εκχωρήσετε μια άδεια χρήσης μέσω: Κέντρο διαχείρισης του Office ή πύλη Azure.
  
Πρόσθετοι πόροι που θα σας βοηθήσουν να επιλύσετε το πρόβλημα:
  
1. Χρησιμοποιήστε την [πύλη αντιμετώπισης προβλημάτων του Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) για να διαγνώσετε και να επιλύσετε συνηθισμένες αποτυχίες εγγραφής. Εξετάστε [αυτό το έγγραφο](https://docs.microsoft.com/intune/help-desk-operators) για περισσότερες λεπτομέρειες.

2. Εξετάστε [αυτό το έγγραφο](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) για μια λίστα με συνηθισμένα σφάλματα που εμποδίζουν την εγγραφή και τις αναλύσεις σε κάθε μία από αυτές.

3. [Μάθετε πώς μπορείτε να εγγράψετε συσκευές Android στο Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
