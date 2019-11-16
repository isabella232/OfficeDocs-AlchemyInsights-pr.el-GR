---
title: Αντιμετώπιση προβλημάτων πρόσβασης δεν επιτρέπεται μηνύματα στο OneDrive για επιχειρηματικές τοποθεσίες
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 3c40ad76a8961a3d0b4963483291c2a1364c51d3
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 11/15/2019
ms.locfileid: "37766711"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Αντιμετώπιση προβλημάτων πρόσβασης δεν επιτρέπεται μηνύματα στο OneDrive για επιχειρηματικές τοποθεσίες

Αυτό το ζήτημα παρουσιάζεται συχνότερα όταν ένας χρήστης διαγράφεται και δημιουργείται ξανά με το ίδιο κύριο όνομα χρήστη (UPN). Ο νέος λογαριασμός δημιουργείται χρησιμοποιώντας μια διαφορετική τιμή PUID (μοναδικό αναγνωριστικό διαβατηρίου). Όταν ο χρήστης προσπαθεί να αποκτήσει πρόσβαση σε μια συλλογή τοποθεσιών ή το OneDrive, ο χρήστης έχει ένα εσφαλμένο PUID. Ένα δεύτερο σενάριο περιλαμβάνει συγχρονισμό καταλόγων με μια οργανωτική μονάδα Active Directory (OU). Εάν οι χρήστες έχουν ήδη εισέλθει στο SharePoint και, στη συνέχεια, μετακινούνται σε μια διαφορετική οργανική μονάδα και να συγχρονίσετε ξανά με το SharePoint, ενδέχεται να αντιμετωπίσετε αυτό το ζήτημα.

1. Για να επιλύσετε αυτό το ζήτημα, πρέπει να επαναφέρετε το αρχικό UPN με τα βήματα του άρθρου, [επαναφέρετε ένα χρήστη στο Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).
2. Εάν δεν μπορείτε να επαναφέρετε τον αρχικό χρήστη, θα πρέπει να καταργήσετε τον παλιό χρήστη από την τοποθεσία του OneDrive χρησιμοποιώντας αυτά τα βήματα, [καταργήστε ένα χρήστη από τη λίστα πληροφοριών χρήστη](). 
3. Μετά από αυτό, μπορείτε να επαληθεύσετε ότι ο χρήστης έχει δικαιώματα διαχειριστή στην τοποθεσία του OneDrive, ακολουθώντας τα βήματα για να [προσθέσετε διαχειριστή για το OneDrive ενός χρήστη](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)

Για περισσότερες πληροφορίες σχετικά με τα επίπεδα δικαιωμάτων, ανατρέξτε στο άρθρο, [κατανόηση των επιπέδων δικαιωμάτων στο SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
