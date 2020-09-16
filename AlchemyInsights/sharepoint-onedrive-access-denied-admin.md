---
title: Αντιμετώπιση προβλημάτων σε μηνύματα που δεν επιτρέπονται
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 22f5966fdae563c44affb7d0447787a4ee0aca93
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767662"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Αντιμετώπιση προβλημάτων με τα μηνύματα που δεν επιτρέπεται στην Access στο κέντρο διαχείρισης του SharePoint/OneDrive

Εάν λαμβάνετε ένα μήνυμα απόρριψης πρόσβασης όταν προσπαθείτε να μεταβείτε σε ένα κέντρο διαχείρισης του SharePoint/OneDrive, βεβαιωθείτε ότι [εκχωρείτε μια άδεια χρήσης στο χρήστη](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). Εάν ο χρήστης έχει άδεια χρήσης, θα πρέπει επίσης να βεβαιωθείτε ότι του έχει [ανατεθεί ρόλος διαχειριστή](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) ο οποίος μπορεί να αποκτήσει πρόσβαση στα κέντρα διαχείρισης.

Αυτό το πρόβλημα μπορεί επίσης να προκύψει όταν ένας χρήστης διαγραφεί και δημιουργηθεί εκ νέου με το ίδιο κύριο όνομα χρήστη (UPN). Ο νέος λογαριασμός δημιουργείται χρησιμοποιώντας μια διαφορετική τιμή PUID (Passport Unique ID). Όταν ο χρήστης προσπαθήσει να αποκτήσει πρόσβαση σε μια συλλογή τοποθεσιών ή στο OneDrive, ο χρήστης έχει εσφαλμένο PUID. Ένα δεύτερο σενάριο περιλαμβάνει τον συγχρονισμό καταλόγων με μια οργανική μονάδα της υπηρεσίας καταλόγου Active Directory (OU). Εάν οι χρήστες έχουν ήδη εισέλθει στο SharePoint και, στη συνέχεια, μετακινηθούν σε διαφορετική οργανική μονάδα και επανασυγχρονιστούν με το SharePoint, ενδέχεται να αντιμετωπίσουν αυτό το πρόβλημα.

Για να επιλύσετε αυτό το πρόβλημα, θα πρέπει να επαναφέρετε το αρχικό UPN με τα βήματα του άρθρου, να [επαναφέρετε ένα χρήστη στο Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).

Σημείωση: Εάν ένα κέντρο διαχείρισης του OneDrive ή του SharePoint δεν είναι διαθέσιμο σε πολλούς χρήστες που είχαν προηγουμένως πρόσβαση, μπορεί να υπάρχει κάποιο πρόβλημα προσωρινής υπηρεσίας.  [Επιλέξτε τον πίνακα εργαλείων εύρυθμης λειτουργίας υπηρεσίας](https://portal.office.com/adminportal/home#/servicehealth).


