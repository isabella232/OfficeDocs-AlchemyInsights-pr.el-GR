---
title: Αντιμετώπιση προβλημάτων με την εγγραφή συσκευών Android στο Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 08620a44dcf693482c65ff05e19f11870f67afbe
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830942"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Αντιμετώπιση προβλημάτων με την εγγραφή συσκευών Android στο Microsoft Intune

Εξετάστε τους πόρους που αναφέρονται παρακάτω για να επιλύσετε το πρόβλημά σας τώρα.
  
Ορισμένα συνήθη προβλήματα και βήματα επίλυσης:
  
 **Σφάλμα "Συσκευή χωρίς κρυπτογράφηση" στην εταιρική πύλη:** Οι νεότερες εκδόσεις του Android, ιδιαίτερα ξεκινώντας από τη v7.0, απαιτούν κωδικό πρόσβασης εκκίνησης για να βεβαιωθούν ότι η συσκευή σας είναι πλήρως κρυπτογραφημένη. Οι συνηθισμένες λύσεις είναι να ενεργοποιήσετε μια καρφίτσα εκκίνησης ή να κρυπτογραφήσετε πλήρως τη συσκευή. Διαβάστε [αυτό το έγγραφο](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) για περισσότερες πληροφορίες.
  
 Οι συσκευές δεν μπορούν να μεταδοτούν με την υπηρεσία Intune ή να εμφανίζονται **ως "Ανθυγιεινά" στην κονσόλα διαχείρισης Intune:** Ορισμένες συσκευές Samsung 4.4 και 5.5 ενδέχεται να μην έχουν έλεγχο της υπηρεσίας. Υπάρχουν 3 πιθανές λύσεις σε αυτό το πρόβλημα:
  
1. Ανοίξτε με μη αυτόματο τρόπο την εφαρμογή Εταιρική πύλη Intune, η οποία θα ξεκινήσει αυτόματα ένα συγχρονισμό συσκευής.

2. Ενημερώστε τη συσκευή σε Android 6.0 ή υψηλότερη έκδοση.

3. Απενεργοποιήστε το Samsung Smart Manager από τη διαχείριση της εταιρικής πύλης Intune. Διαβάστε [αυτό το έγγραφο](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) για περισσότερες λεπτομέρειες σχετικά με αυτά τα ζητήματα και τις λύσεις.

 **Σφάλμα "Μη έγκυρος τύπος** άδειας χρήσης" ή "Μη αναγνωρισμένο όνομα **χρήστη":** Πρέπει να εκχωρηθεί στο χρήστη μια άδεια χρήσης Intune ή EMS. Εξετάστε αυτά τα έγγραφα για να εκχωρήσετε μια άδεια χρήσης μέσω: Του Κέντρου διαχείρισης του Office ή της πύλης Azure.
  
Πρόσθετοι πόροι για την επίλυση του προβλήματος:
  
1. Χρησιμοποιήστε [την Πύλη αντιμετώπισης προβλημάτων intune για](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) να διαγνώσετε και να επιλύσετε συνηθισμένες αποτυχίες εγγραφής. Διαβάστε [αυτό το έγγραφο](https://docs.microsoft.com/intune/help-desk-operators) για περισσότερες λεπτομέρειες.

2. Εξετάστε [αυτό το έγγραφο](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) για μια λίστα με συνήθη σφάλματα που εμποδίζουν την εγγραφή και τις λύσεις για το καθένα.

3. [Μάθετε πώς μπορείτε να εγγράψετε συσκευές Android στο Microsoft Intune.](https://docs.microsoft.com/intune/android-enroll)
