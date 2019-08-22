---
title: Αντιμετώπιση προβλημάτων σχετικά με την εγγραφή Android συσκευές στη Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: 1e1d50c31df588a3416d758d40fbd7bde3f73b21
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36500071"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Αντιμετώπιση προβλημάτων σχετικά με την εγγραφή Android συσκευές στη Microsoft Intune

Εξετάστε τους πόρους που αναφέρονται παρακάτω για να επιλύσετε το θέμα σας τώρα.
  
Ορισμένα συνηθισμένα προβλήματα και βήματα επίλυσης:
  
 **Συσκευή δεν κρυπτογραφούνται σφάλμα στο εμπόριο εταιρείας:** Νεότερες εκδόσεις του Android, ιδίως από v7.0, απαιτούν έναν κωδικό πρόσβασης εκκίνησης για να βεβαιωθείτε ότι η συσκευή σας είναι πλήρως κρυπτογραφημένη. Συνήθεις λύσεις πρόκειται να ενεργοποιήσετε ένα pin εκκίνησης ή πλήρη κρυπτογράφηση της συσκευής. Αναθεωρήστε [αυτό το έγγραφο](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) για περισσότερες πληροφορίες.
  
 **Συσκευές αδυνατούν να ενημερωθείτε από την υπηρεσία Intune ή να εμφανιστεί ως "Unhealthy" στην κονσόλα διαχείρισης του Intune:** Ορισμένα Samsung 4.4 και 5.5 συσκευές δεν μπορούν να ελέγχουν στην υπηρεσία. Υπάρχουν 3 πιθανές λύσεις για αυτό το ζήτημα:
  
1. Ανοίξτε με μη αυτόματο τρόπο το app Intune εταιρεία πύλη, που θα ξεκινήσει αυτόματα την συσκευή συγχρονισμού.

2. Ενημερώστε τη συσκευή με Android 6.0 ή νεότερη έκδοση.

3. Απενεργοποίηση Samsung έξυπνη διαχείριση με τη διαχείριση της πύλης εταιρείας Intune. Εξετάστε [αυτό το έγγραφο](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) για περισσότερες λεπτομέρειες σχετικά με αυτά τα θέματα και λύσεις.

 **Χρήστης άδεια τύπου δεν είναι έγκυρος** ή **χρήστη όνομα δεν αναγνωρίζεται σφάλμα:** ο χρήστης θα πρέπει να αντιστοιχιστεί μια άδεια Intune ή EMS. Εξετάστε αυτά τα έγγραφα για να αναθέσετε μια άδεια χρήσης μέσω: Κέντρο διαχείρισης του Office ή Azure πύλης.
  
Πρόσθετους πόρους για να σας βοηθήσουν να επιλύσετε το ζήτημα:
  
1. Χρησιμοποιήστε [Πύλη του Intune αντιμετώπιση προβλημάτων](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) για να διαγνώσετε και να επιλύσετε συνηθισμένα σφάλματα εγγραφής. Αναθεωρήστε [αυτό το έγγραφο](https://docs.microsoft.com/intune/help-desk-operators) για περισσότερες λεπτομέρειες.

2. Αναθεωρήστε [αυτό το έγγραφο](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) για μια λίστα κοινών σφαλμάτων που εμποδίζουν εγγραφής και λύσεις για κάθε μία.

3. [Μάθετε πώς μπορείτε να εγγραφείτε Android συσκευές στη Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
