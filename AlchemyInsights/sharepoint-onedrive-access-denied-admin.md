---
title: Αντιμετώπιση προβλημάτων μηνυμάτων άρνησης πρόσβασης
ms.author: pebaum
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 4e6fdc6fbf745d1702bf1a7b3474ac82f6662305
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36751276"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Αντιμετώπιση προβλημάτων με τα μηνύματα άρνησης πρόσβασης στο κέντρο διαχείρισης του SharePoint/OneDrive

Εάν λαμβάνετε ένα μήνυμα άρνησης πρόσβασης κατά την προσπάθεια αναζήτησης σε ένα κέντρο διαχείρισης του SharePoint/OneDrive, βεβαιωθείτε ότι έχετε [εκχωρήσει μια άδεια χρήσης στο χρήστη](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One). Εάν ο χρήστης έχει άδεια χρήσης, θα πρέπει επίσης να βεβαιωθείτε ότι τους έχει [ανατεθεί ένας ρόλος διαχειριστή](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) που μπορεί να αποκτήσει πρόσβαση στα κέντρα διαχείρισης.

Αυτό το ζήτημα μπορεί επίσης να προκύψει όταν ένας χρήστης διαγράφεται και δημιουργείται ξανά με το ίδιο κύριο όνομα χρήστη (UPN). Ο νέος λογαριασμός δημιουργείται χρησιμοποιώντας μια διαφορετική τιμή PUID (μοναδικό αναγνωριστικό διαβατηρίου). Όταν ο χρήστης προσπαθεί να αποκτήσει πρόσβαση σε μια συλλογή τοποθεσιών ή το OneDrive, ο χρήστης έχει ένα εσφαλμένο PUID. Ένα δεύτερο σενάριο περιλαμβάνει συγχρονισμό καταλόγων με μια οργανωτική μονάδα Active Directory (OU). Εάν οι χρήστες έχουν ήδη εισέλθει στο SharePoint και, στη συνέχεια, μετακινούνται σε μια διαφορετική οργανική μονάδα και να συγχρονίσετε ξανά με το SharePoint, ενδέχεται να αντιμετωπίσετε αυτό το ζήτημα.

Για να επιλύσετε αυτό το ζήτημα, θα πρέπει να επαναφέρετε το αρχικό UPN με τα βήματα του άρθρου, [επαναφέρετε ένα χρήστη στο Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

Σημείωση: Εάν ένα OneDrive ή το κέντρο διαχείρισης του SharePoint δεν είναι διαθέσιμο σε πολλούς χρήστες που είχαν προηγουμένως πρόσβαση, ενδέχεται να υπάρχει ένα ζήτημα προσωρινής υπηρεσίας.  [Ελέγξτε τον πίνακα εργαλείων εύρυθμης λειτουργίας υπηρεσίας](https://portal.office.com/adminportal/home#/servicehealth).


