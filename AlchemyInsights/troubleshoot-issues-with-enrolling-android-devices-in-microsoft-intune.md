---
title: Αντιμετώπιση προβλημάτων με την εγγραφή συσκευών Android στο Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: bd6d278ebf6cca7fb6e4ac1049deae600b516707
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759620"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Αντιμετώπιση προβλημάτων με την εγγραφή συσκευών Android στο Microsoft Intune

Εξετάστε τους πόρους που παρατίθενται παρακάτω για να επιλύσετε το ζήτημά σας τώρα.
  
Ορισμένα συνηθισμένα ζητήματα και βήματα επίλυσης:
  
 **Η συσκευή δεν είναι κρυπτογραφημένο σφάλμα στην εταιρική πύλη:** Οι νεότερες εκδόσεις του Android, ιδιαίτερα ξεκινώντας από το v7.0, απαιτούν έναν κωδικό πρόσβασης εκκίνησης για να βεβαιωθείτε ότι η συσκευή σας είναι πλήρως κρυπτογραφημένη. Οι συνήθεις λύσεις είναι να ενεργοποιήσετε μια καρφίτσα εκκίνησης ή να κρυπτογραφήσετε πλήρως τη συσκευή. Εξετάστε [αυτό το έγγραφο](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) για περισσότερες πληροφορίες.
  
 **Οι συσκευές δεν μπορούν να κάνουν μεταβίβαση ελέγχου με την υπηρεσία Intune ή να εμφανίζονται ως "Ανθυγιεινά" στην κονσόλα διαχείρισης Intune:** Ορισμένες συσκευές Samsung 4.4 και 5.5 ενδέχεται να μην κάνουν check-in στην υπηρεσία. Υπάρχουν 3 πιθανές λύσεις σε αυτό το ζήτημα:
  
1. Ανοίξτε με μη αυτόματο τρόπο την εφαρμογή Intune Company Portal, η οποία θα ξεκινήσει αυτόματα ένα συγχρονισμό συσκευών.

2. Ενημερώστε τη συσκευή σε Android 6.0 ή νεότερη έκδοση.

3. Απενεργοποιήστε το Samsung Smart Manager από τη διαχείριση της πύλης της εταιρείας Intune. Εξετάστε [το παρόν έγγραφο](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) για περισσότερες λεπτομέρειες σχετικά με αυτά τα θέματα και τα ψηφίσματα.

 **Ο τύπος άδειας χρήσης δεν είναι έγκυρος** ή **το όνομα χρήστη που δεν αναγνωρίζεται σφάλμα:** Ο χρήστης πρέπει να του εκχωρηθεί μια άδεια χρήσης Intune ή EMS. Εξετάστε αυτά τα έγγραφα για να εκχωρήσετε μια άδεια χρήσης μέσω: Κέντρο διαχείρισης του Office ή πύλη Azure.
  
Πρόσθετοι πόροι που θα σας βοηθήσουν να επιλύσετε το ζήτημά σας:
  
1. Χρησιμοποιήστε την [πύλη αντιμετώπισης προβλημάτων intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) για να διαγνώσετε και να επιλύσετε συνήθεις αποτυχίες εγγραφής. Εξετάστε [αυτό το έγγραφο](https://docs.microsoft.com/intune/help-desk-operators) για περισσότερες λεπτομέρειες.

2. Εξετάστε [αυτό το έγγραφο](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) για μια λίστα συνηθισμένων σφαλμάτων που εμποδίζουν την εγγραφή και τις λύσεις σε κάθε έγγραφο.

3. [Μάθετε πώς μπορείτε να εγγράψετε συσκευές Android στο Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
