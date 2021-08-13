---
title: Αντιμετώπιση προβλημάτων κατά την οποία η Access απέρριψε μηνύματα OneDrive για επιχειρήσεις τοποθεσίες
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
ms.openlocfilehash: fc4a2bd7dcc74f5f05e8b709e4bc3eac6ed445d6e2ea9ede698abbc8667723ce
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957793"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Αντιμετώπιση προβλημάτων κατά την οποία η Access απέρριψε μηνύματα OneDrive για επιχειρήσεις τοποθεσίες

Αυτό το πρόβλημα παρουσιάζεται πιο συχνά όταν ένας χρήστης διαγράφεται και δημιουργείται εκ νέο με το ίδιο κύριο όνομα χρήστη (UPN). Ο νέος λογαριασμός δημιουργείται χρησιμοποιώντας μια διαφορετική τιμή PUID (Μοναδικό αναγνωριστικό διαβατηρίου). Όταν ο χρήστης προσπαθεί να αποκτήσει πρόσβαση σε μια συλλογή τοποθεσιών ή OneDrive, ο χρήστης έχει εσφαλμένο PUID. Ένα δεύτερο σενάριο αφορά το συγχρονισμό καταλόγου με μια εταιρική μονάδα υπηρεσίας καταλόγου Active Directory (OU). Εάν οι χρήστες έχουν ήδη εισέλθει στο SharePoint και, στη συνέχεια, μετακινηθούν σε διαφορετική OU και επανασυγχρονιστεί με το SharePoint, ενδέχεται να αντιμετωπίσετε αυτό το πρόβλημα.

1. Για να επιλύσετε αυτό το πρόβλημα, θα πρέπει να επαναφέρετε το αρχικό UPN με τα βήματα που αναφέρονται στο άρθρο, [επαναφέρετε ένα χρήστη στο Microsoft 365.](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)
2. Εάν δεν μπορείτε να επαναφέρετε τον αρχικό χρήστη, θα πρέπει να καταργήσετε τον παλιό χρήστη από την τοποθεσία OneDrive χρησιμοποιώντας αυτά τα βήματα, καταργήστε ένα χρήστη [από τη λίστα πληροφοριών χρήστη.]() 
3. Αφού γίνει αυτό, μπορείτε να επαληθεύσετε ότι ο χρήστης έχει δικαιώματα διαχειριστή στην τοποθεσία OneDrive, ακολουθώντας τα βήματα για την προσθήκη [διαχειριστών](https://docs.microsoft.com/sharepoint/manage-user-profiles) για τα δικαιώματα OneDrive

Για περισσότερες πληροφορίες σχετικά με τα επίπεδα δικαιωμάτων, ανατρέξτε στο άρθρο [,Κατανόηση των επιπέδων δικαιωμάτων SharePoint.](https://docs.microsoft.com/sharepoint/understanding-permission-levels)
