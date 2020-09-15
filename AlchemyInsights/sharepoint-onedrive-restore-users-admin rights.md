---
title: Αντιμετώπιση προβλημάτων στα μηνύματα που δεν επιτρέπονται στο OneDrive για επιχειρηματικές τοποθεσίες
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9001cf0b7d9f1f05a2ecedca2c3137dd1b8a1c38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670616"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Αντιμετώπιση προβλημάτων στα μηνύματα που δεν επιτρέπονται στο OneDrive για επιχειρηματικές τοποθεσίες

Αυτό το πρόβλημα παρουσιάζεται συχνότερα όταν ένας χρήστης διαγράφεται και δημιουργείται εκ νέου με το ίδιο κύριο όνομα χρήστη (UPN). Ο νέος λογαριασμός δημιουργείται χρησιμοποιώντας μια διαφορετική τιμή PUID (Passport Unique ID). Όταν ο χρήστης προσπαθήσει να αποκτήσει πρόσβαση σε μια συλλογή τοποθεσιών ή στο OneDrive, ο χρήστης έχει εσφαλμένο PUID. Ένα δεύτερο σενάριο περιλαμβάνει τον συγχρονισμό καταλόγων με μια οργανική μονάδα της υπηρεσίας καταλόγου Active Directory (OU). Εάν οι χρήστες έχουν ήδη εισέλθει στο SharePoint και, στη συνέχεια, μετακινηθούν σε διαφορετική οργανική μονάδα και επανασυγχρονιστούν με το SharePoint, ενδέχεται να αντιμετωπίσουν αυτό το πρόβλημα.

1. Για να επιλύσετε αυτό το πρόβλημα, θα πρέπει να επαναφέρετε το αρχικό UPN με τα βήματα του άρθρου, να [επαναφέρετε ένα χρήστη στο Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).
2. Εάν δεν μπορείτε να επαναφέρετε τον αρχικό χρήστη, θα πρέπει να καταργήσετε τον παλιό χρήστη από την τοποθεσία του OneDrive, χρησιμοποιώντας αυτά τα βήματα, να [καταργήσετε ένα χρήστη από τη λίστα πληροφοριών χρήστη](). 
3. Αφού ολοκληρωθεί αυτή η ενέργεια, μπορείτε να επαληθεύσετε ότι ο χρήστης έχει δικαιώματα διαχειριστή στην τοποθεσία του OneDrive, ακολουθώντας τα βήματα για την [Προσθήκη του διαχειριστή για το OneDrive ενός χρήστη](https://docs.microsoft.com/sharepoint/manage-user-profiles)

Για περισσότερες πληροφορίες σχετικά με τα επίπεδα δικαιωμάτων, ανατρέξτε στο άρθρο [κατανόηση των επιπέδων δικαιωμάτων στο SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
