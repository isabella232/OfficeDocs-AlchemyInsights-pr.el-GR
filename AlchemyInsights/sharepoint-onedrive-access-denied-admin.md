---
title: Αντιμετώπιση προβλημάτων για μηνύματα που δεν επιτρέπεται να έχουν πρόσβαση
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3189fa61d28253569278024d4191ee63b917509f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707954"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Αντιμετώπιση προβλημάτων κατά την πρόσβαση σε μηνύματα που δεν επιτρέπεται στο Sharepoint/Κέντρο διαχείρισης του OneDrive

Εάν λαμβάνετε ένα μήνυμα άρνησης πρόσβασης όταν προσπαθείτε να περιηγηθείτε σε ένα Κέντρο διαχείρισης του Sharepoint/OneDrive, βεβαιωθείτε ότι έχετε εκχωρήσει μια άδεια χρήσης [στο χρήστη.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users) Εάν ο χρήστης έχει μια άδεια χρήσης, [](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) θα πρέπει επίσης να βεβαιωθείτε ότι έχει εκχωρηθεί ένας ρόλος διαχειριστή στον οποίο έχει πρόσβαση στα κέντρα διαχείρισης.

Αυτό το πρόβλημα μπορεί επίσης να προκύψει όταν ένας χρήστης διαγραφεί και δημιουργηθεί εκ νέα με το ίδιο κύριο όνομα χρήστη (UPN). Ο νέος λογαριασμός δημιουργείται χρησιμοποιώντας μια διαφορετική τιμή PUID (Αναγνωριστικό μοναδικού διαβατηρίου). Όταν ο χρήστης προσπαθεί να αποκτήσει πρόσβαση σε μια συλλογή τοποθεσιών ή στο OneDrive του, ο χρήστης έχει ένα εσφαλμένο PUID. Ένα δεύτερο σενάριο περιλαμβάνει το συγχρονισμό καταλόγου με μια οργανική μονάδα (OU) της υπηρεσίας καταλόγου Active Directory. Εάν οι χρήστες έχουν ήδη εισέλθει στο SharePoint και, στη συνέχεια, μετακινηθούν σε διαφορετική OU και έχουν επανασυγχρονιστεί με το SharePoint, ενδέχεται να αντιμετωπίσετε αυτό το πρόβλημα.

Για να επιλύσετε αυτό το ζήτημα, θα πρέπει να επαναφέρετε το αρχικό UPN με τα βήματα που αναφέρονται στο άρθρο "Επαναφορά [χρήστη στο Microsoft 365".](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)

Σημείωση: Εάν ένα Κέντρο διαχείρισης του OneDrive ή του SharePoint δεν είναι διαθέσιμο για πολλούς χρήστες που είχαν προηγουμένως πρόσβαση, ενδέχεται να υπάρχει ένα προσωρινό ζήτημα υπηρεσίας.  [Ελέγξτε τον πίνακα εργαλείων της υγείας των υπηρεσιών.](https://portal.office.com/adminportal/home#/servicehealth)


