---
title: Αντιμετώπιση προβλημάτων μηνυμάτων που δεν επιτρέπεται η πρόσβαση σε τοποθεσίες του OneDrive για επιχειρήσεις
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 95bd46e8b7a6006f3735612d9a5602fb2b2a283b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511184"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Αντιμετώπιση προβλημάτων μηνυμάτων που δεν επιτρέπεται η πρόσβαση σε τοποθεσίες του OneDrive για επιχειρήσεις

Αυτό το ζήτημα παρουσιάζεται συχνότερα όταν ένας χρήστης διαγράφεται και δημιουργείται ξανά με το ίδιο κύριο όνομα χρήστη (UPN). Ο νέος λογαριασμός δημιουργείται χρησιμοποιώντας μια διαφορετική τιμή PUID (Passport Unique ID). Όταν ο χρήστης προσπαθεί να αποκτήσει πρόσβαση σε μια συλλογή τοποθεσιών ή το OneDrive, ο χρήστης έχει εσφαλμένο PUID. Ένα δεύτερο σενάριο περιλαμβάνει συγχρονισμό καταλόγου με μια οργανωτική μονάδα της υπηρεσίας καταλόγου Active Directory (OU). Εάν οι χρήστες έχουν ήδη εισέλθει στο SharePoint και, στη συνέχεια, μετακινούνται σε διαφορετική οργανική μονάδα και επανασυγχρονίζονται με το SharePoint, ενδέχεται να αντιμετωπίσουν αυτό το ζήτημα.

1. Για να επιλύσετε αυτό το ζήτημα, θα πρέπει να επαναφέρετε το αρχικό UPN με τα βήματα του άρθρου, [Επαναφορά ενός χρήστη στο Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).
2. Εάν δεν μπορείτε να επαναφέρετε τον αρχικό χρήστη, θα πρέπει να καταργήσετε τον παλιό χρήστη από την τοποθεσία του OneDrive χρησιμοποιώντας αυτά τα βήματα, [καταργήστε ένα χρήστη από τη λίστα πληροφοριών χρήστη](). 
3. Αφού γίνει αυτό, μπορείτε να επαληθεύσετε ότι ο χρήστης έχει δικαιώματα διαχειριστή στην τοποθεσία του OneDrive, ακολουθώντας τα βήματα για την [προσθήκη διαχειριστή για το OneDrive ενός χρήστη](https://docs.microsoft.com/sharepoint/manage-user-profiles)

Για περισσότερες πληροφορίες σχετικά με τα επίπεδα δικαιωμάτων, ανατρέξτε στο άρθρο , [Κατανόηση των επιπέδων δικαιωμάτων στο SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
