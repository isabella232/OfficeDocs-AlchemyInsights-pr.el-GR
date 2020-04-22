---
title: Αντιμετώπιση προβλημάτων μηνυμάτων που δεν επιτρέπεται η πρόσβαση
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 82e11458529b8a49e583b1a6963a51e2a466bfd6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758436"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Αντιμετώπιση προβλημάτων μηνυμάτων που δεν επιτρέπεται πρόσβασης στο Κέντρο διαχείρισης του Sharepoint/OneDrive

Εάν λαμβάνετε ένα μήνυμα που δεν επιτρέπεται από την πρόσβαση κατά την προσπάθεια αναζήτησης σε ένα Κέντρο διαχείρισης του Sharepoint/OneDrive, βεβαιωθείτε ότι [εκχωρείτε μια άδεια χρήσης στο χρήστη](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One). Εάν ο χρήστης έχει άδεια χρήσης, θα πρέπει επίσης να βεβαιωθείτε ότι του [έχει ανατεθεί ένας ρόλος διαχειριστή](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) που μπορεί να έχει πρόσβαση στα κέντρα διαχείρισης.

Αυτό το ζήτημα μπορεί επίσης να προκύψει όταν ένας χρήστης διαγράφεται και δημιουργείται ξανά με το ίδιο κύριο όνομα χρήστη (UPN). Ο νέος λογαριασμός δημιουργείται χρησιμοποιώντας μια διαφορετική τιμή PUID (Passport Unique ID). Όταν ο χρήστης προσπαθεί να αποκτήσει πρόσβαση σε μια συλλογή τοποθεσιών ή το OneDrive, ο χρήστης έχει εσφαλμένο PUID. Ένα δεύτερο σενάριο περιλαμβάνει συγχρονισμό καταλόγου με μια οργανωτική μονάδα της υπηρεσίας καταλόγου Active Directory (OU). Εάν οι χρήστες έχουν ήδη εισέλθει στο SharePoint και, στη συνέχεια, μετακινούνται σε διαφορετική οργανική μονάδα και επανασυγχρονίζονται με το SharePoint, ενδέχεται να αντιμετωπίσουν αυτό το ζήτημα.

Για να επιλύσετε αυτό το ζήτημα, θα πρέπει να επαναφέρετε το αρχικό UPN με τα βήματα του άρθρου, [Επαναφορά ενός χρήστη στο Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

Σημείωση: Εάν ένα κέντρο διαχείρισης του OneDrive ή του SharePoint δεν είναι διαθέσιμο σε πολλούς χρήστες που είχαν προηγουμένως πρόσβαση, ενδέχεται να υπάρχει ένα ζήτημα προσωρινής υπηρεσίας.  [Ελέγξτε τον πίνακα εργαλείων εύρυθμης λειτουργίας υπηρεσίας](https://portal.office.com/adminportal/home#/servicehealth).


