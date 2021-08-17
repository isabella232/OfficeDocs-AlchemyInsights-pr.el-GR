---
title: Αντιμετώπιση προβλημάτων με τα μηνύματα που δεν επιτρέπεται να έχουν πρόσβαση
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 9acde72f82a27c9f2faa2cf4d0417374aa5a294234da96080dc0498d07639248
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54085228"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Αντιμετώπιση προβλημάτων των μηνυμάτων που δεν επιτρέπεται να έχουν πρόσβαση στο Sharepoint/OneDrive Κέντρο διαχείρισης

Εάν λαμβάνετε ένα μήνυμα άρνησης πρόσβασης κατά την προσπάθεια περιήγησης σε ένα Κέντρο διαχείρισης του Sharepoint/OneDrive, βεβαιωθείτε ότι έχετε εκχωρήσει μια άδεια [χρήσης στο χρήστη.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users) Εάν ο χρήστης έχει μια άδεια χρήσης, θα πρέπει επίσης να βεβαιωθείτε ότι του έχει εκχωρηθεί ένας ρόλος [διαχειριστή](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) που μπορεί να έχει πρόσβαση στα κέντρα διαχείρισης.

Αυτό το πρόβλημα μπορεί επίσης να προκύψει όταν ένας χρήστης διαγραφεί και δημιουργηθεί εκ νέο με το ίδιο κύριο όνομα χρήστη (UPN). Ο νέος λογαριασμός δημιουργείται χρησιμοποιώντας μια διαφορετική τιμή PUID (Μοναδικό αναγνωριστικό διαβατηρίου). Όταν ο χρήστης προσπαθεί να αποκτήσει πρόσβαση σε μια συλλογή τοποθεσιών ή OneDrive, ο χρήστης έχει εσφαλμένο PUID. Ένα δεύτερο σενάριο αφορά το συγχρονισμό καταλόγου με μια εταιρική μονάδα υπηρεσίας καταλόγου Active Directory (OU). Εάν οι χρήστες έχουν ήδη εισέλθει στο SharePoint και, στη συνέχεια, μετακινηθούν σε διαφορετική OU και επανασυγχρονιστεί με το SharePoint, ενδέχεται να αντιμετωπίσετε αυτό το πρόβλημα.

Για να επιλύσετε αυτό το πρόβλημα, θα πρέπει να επαναφέρετε το αρχικό UPN με τα βήματα που αναφέρονται στο άρθρο, επαναφορά [ενός χρήστη Microsoft 365.](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)

Σημείωση: Εάν ένα OneDrive ή SharePoint διαχείρισης δεν είναι διαθέσιμο σε πολλούς χρήστες που είχαν προηγουμένως πρόσβαση, ενδέχεται να υπάρχει ένα προσωρινό πρόβλημα υπηρεσίας.  [Ελέγξτε τον πίνακα εργαλείων της υπηρεσίας υγείας.](https://portal.office.com/adminportal/home#/servicehealth)


