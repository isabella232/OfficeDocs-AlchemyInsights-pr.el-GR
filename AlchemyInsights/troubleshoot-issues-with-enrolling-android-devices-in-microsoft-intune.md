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
ms.openlocfilehash: cc8c68a1e838f67c4510002b2c7ff5294a4649fe
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708998"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Αντιμετώπιση προβλημάτων με την εγγραφή συσκευών Android στο Microsoft Intune

Εξετάστε τους πόρους που παρατίθενται παρακάτω για να επιλύσετε το πρόβλημά σας τώρα.
  
Ορισμένα συνήθη προβλήματα και βήματα επίλυσης:
  
 **Σφάλμα "Η συσκευή δεν είναι κρυπτογραφημένο" στην εταιρική πύλη:** Για τις νεότερες εκδόσεις του Android, ιδιαίτερα όταν ξεκινούν με v7.0, απαιτείται κωδικός πρόσβασης εκκίνησης για να βεβαιωθείτε ότι η συσκευή σας είναι πλήρως κρυπτογραφημένη. Συνήθεις λύσεις είναι να ενεργοποιήσετε μια καρφίτσα εκκίνησης ή να κρυπτογραφήσετε πλήρως τη συσκευή. Διαβάστε [αυτό το έγγραφο](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) για περισσότερες πληροφορίες.
  
 Ο έλεγχος της υπηρεσίας Intune στις συσκευές αποτυγχάνουν ή εμφανίζεται ως **"Μη εύρυθμη λειτουργία" στην κονσόλα διαχείρισης του Intune:** Ορισμένες συσκευές Samsung 4.4 και 5.5 ενδέχεται να μην check into the service. Υπάρχουν 3 πιθανές λύσεις σε αυτό το πρόβλημα:
  
1. Ανοίξτε με μη αυτόματο τρόπο την εφαρμογή Εταιρική πύλη του Intune, η οποία θα ξεκινήσει αυτόματα έναν συγχρονισμό συσκευής.

2. Ενημερώστε τη συσκευή σε Android 6.0 ή υψηλότερη έκδοση.

3. Απενεργοποιήστε το Samsung Smart Manager από τη διαχείριση της εταιρικής πύλης Intune. Διαβάστε [αυτό το έγγραφο](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) για περισσότερες λεπτομέρειες σχετικά με αυτά τα ζητήματα και τις λύσεις.

 **Σφάλμα "Μη έγκυρος τύπος** **άδειας χρήσης"** ή "Δεν αναγνωρίζεται το όνομα χρήστη": Στο χρήστη πρέπει να εκχωρηθεί μια άδεια χρήσης Intune ή EMS. Εξετάστε αυτά τα έγγραφα για να εκχωρήσετε μια άδεια χρήσης μέσω: Κέντρο διαχείρισης του Office ή πύλη Azure.
  
Πρόσθετοι πόροι που θα σας βοηθήσουν να επιλύσετε το πρόβλημα:
  
1. Χρησιμοποιήστε [την Πύλη αντιμετώπισης προβλημάτων του Intune για](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) τη διάγνωση και την επίλυση συνηθισμένων αποτυχιών εγγραφής. Διαβάστε [αυτό το έγγραφο](https://docs.microsoft.com/intune/help-desk-operators) για περισσότερες λεπτομέρειες.

2. Εξετάστε [αυτό το έγγραφο](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) για μια λίστα με συνηθισμένα σφάλματα που εμποδίζουν την εγγραφή και την επίλυση του καθένα.

3. [Μάθετε πώς μπορείτε να εγγράψετε συσκευές Android στο Microsoft Intune.](https://docs.microsoft.com/intune/android-enroll)
