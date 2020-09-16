---
title: Κέντρο διαχείρισης του Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: bb0d757aab05132ff7169ce75009d7012b9a836c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670364"
---
# <a name="teams-admin-center"></a>Κέντρο διαχείρισης του Teams

Μάθετε σχετικά με τη διαχείριση του Teams με το [Κέντρο διαχείρισης του Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

Εάν δεν μπορείτε να αποκτήσετε πρόσβαση στο κέντρο διαχείρισης του Teams, ελέγξτε τα ακόλουθα στοιχεία:

- Βεβαιωθείτε ότι έχετε επιτρέψει στις κατάλληλες [διευθύνσεις IP και διευθύνσεις URL του Office 365](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) σε οποιεσδήποτε περιμετρικές συσκευές (τείχος προστασίας, κ. λπ.) ή στους κανόνες τείχους προστασίας στον τοπικό υπολογιστή σας.
- Επαληθεύστε ότι η σύνδεση που χρησιμοποιείτε για να αποκτήσετε πρόσβαση στην πύλη διαχείρισης του Teams συμφωνεί με το όνομα χρήστη που αναγράφεται στην [πύλη διαχείρισης του Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).

Εάν δεν εμφανίζονται χρήστες στο κέντρο διαχείρισης του Teams, ελέγξτε τα ακόλουθα:

- Έχετε δημιουργήσει χρήστες ή έχετε εκχωρήσει άδειες χρήσης τις τελευταίες 24 ώρες; Φροντίστε να περιμένετε τουλάχιστον 24 ώρες πριν ανοίξετε ένα δελτίο υποστήριξης.
- Είστε βέβαιοι ότι έχετε εκχωρήσει κατάλληλες άδειες χρήσης;
- Εάν έχετε μια υπηρεσία καταλόγου Active Directory εσωτερικής εγκατάστασης, επαληθεύστε ότι [η τιμή msRTCSIP-PrimaryUserAddress ή η διεύθυνση SIP στο πεδίο proxyAddresses της τοπικής υπηρεσίας καταλόγου Active Directory είναι μοναδική και η μορφή ταιριάζει](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) με SIP: το**όνομα** χρήστη του χρήστη από το [Κέντρο διαχείρισης του Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).
- Εάν σκοπεύετε να διατηρήσετε μια ανάπτυξη του Skype για επιχειρήσεις Server και να έχετε χρήστες που διαθέτουν εσωτερικές εγκαταστάσεις και online: ακολουθήστε τις επιλογές **"ρύθμιση υβριδικού με ομάδες και Skype για επιχειρήσεις online"** στον πίνακα ελέγχου του Skype για επιχειρήσεις και μετακινήστε τους χρήστες στο Internet.
