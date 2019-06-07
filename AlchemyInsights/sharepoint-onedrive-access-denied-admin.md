---
title: Αντιμετώπιση προβλημάτων σχετικά με μηνύματα που δεν επιτρέπεται η πρόσβαση
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: c204f1889e03886fdfd3d1c760a4a2beb82b0836
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760341"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Αντιμετώπιση προβλημάτων σχετικά με μηνύματα που δεν επιτρέπεται η πρόσβαση στο Κέντρο διαχείρισης του Sharepoint/OneDrive

Εάν λαμβάνετε ένα μήνυμα απαγόρευσης, κατά την προσπάθειά σας να μεταβείτε σε ένα Κέντρο διαχείρισης Sharepoint/OneDrive πρόσβασης, βεβαιωθείτε ότι μπορείτε να [αναθέσετε μια άδεια χρήσης για το χρήστη](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One). Εάν ο χρήστης έχει άδεια χρήσης, θα πρέπει να βρίσκονται [που έχει αντιστοιχιστεί σε έναν ρόλο διαχειριστή](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) που μπορούν να έχουν πρόσβαση στα κέντρα διαχείρισης.

Αυτό το ζήτημα μπορεί να προκύψει, όταν ο χρήστης έχει διαγραφεί και να δημιουργηθεί εκ νέου με το ίδιο κύριο όνομα χρήστη (UPN). Ο νέος λογαριασμός δημιουργείται χρησιμοποιώντας μια διαφορετική τιμή PUID (μοναδικό Αναγνωριστικό Passport). Όταν ο χρήστης προσπαθήσει να αποκτήσει πρόσβαση σε μια συλλογή τοποθεσιών ή τους OneDrive, ο χρήστης έχει μια εσφαλμένη PUID. Ένα δεύτερο σενάριο περιλαμβάνει συγχρονισμού καταλόγου με μια υπηρεσία καταλόγου Active Directory οργανική μονάδα (OU). Εάν οι χρήστες έχουν ήδη εισέλθει στο SharePoint, και στη συνέχεια θα μετακινηθεί σε μια διαφορετική OU και resynced με το SharePoint, αυτά ενδέχεται να αντιμετωπίσετε αυτό το ζήτημα.

Για να επιλύσετε αυτό το ζήτημα, θα πρέπει να επαναφέρετε το αρχικό UPN ακολουθώντας τα βήματα στο άρθρο, [επαναφέρετε ένα χρήστη στο Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

Σημείωση: Εάν ένα κέντρο OneDrive ή διαχείρισης του SharePoint δεν είναι διαθέσιμες σε πολλούς χρήστες που προηγουμένως είχαν πρόσβαση, ίσως υπάρχει κάποιο ζήτημα προσωρινής υπηρεσίας.  [Ελέγξτε τον πίνακα εργαλείων υγείας υπηρεσία](https://portal.office.com/adminportal/home#/servicehealth).


