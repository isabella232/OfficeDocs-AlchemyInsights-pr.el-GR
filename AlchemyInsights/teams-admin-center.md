---
title: Κέντρο διαχείρισης του Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: 4a3a0796cedd81919066d870c5ca99fe2e978cf8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826379"
---
# <a name="teams-admin-center"></a>Κέντρο διαχείρισης του Teams

Μάθετε σχετικά με τη διαχείριση του Teams με το [Κέντρο διαχείρισης του Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

Εάν δεν μπορείτε να αποκτήσετε πρόσβαση στο κέντρο διαχείρισης του Teams, ελέγξτε τα ακόλουθα στοιχεία:

- Βεβαιωθείτε ότι έχετε επιτρέψει στις κατάλληλες [διευθύνσεις IP και διευθύνσεις URL του Office 365](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) σε οποιεσδήποτε περιμετρικές συσκευές (τείχος προστασίας, κ. λπ.) ή στους κανόνες τείχους προστασίας στον τοπικό υπολογιστή σας.
- Επαληθεύστε ότι η σύνδεση που χρησιμοποιείτε για να αποκτήσετε πρόσβαση στην πύλη διαχείρισης του Teams συμφωνεί με το όνομα χρήστη που αναγράφεται στην [πύλη διαχείρισης του Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).

Εάν δεν εμφανίζονται χρήστες στο κέντρο διαχείρισης του Teams, ελέγξτε τα ακόλουθα:

- Έχετε δημιουργήσει χρήστες ή έχετε εκχωρήσει άδειες χρήσης τις τελευταίες 24 ώρες; Φροντίστε να περιμένετε τουλάχιστον 24 ώρες πριν ανοίξετε ένα δελτίο υποστήριξης.
- Είστε βέβαιοι ότι έχετε εκχωρήσει κατάλληλες άδειες χρήσης;
- Εάν έχετε μια υπηρεσία καταλόγου Active Directory εσωτερικής εγκατάστασης, βεβαιωθείτε ότι η τιμή [του msRTCSIP-PrimaryUserAddress ή της διεύθυνσης SIP στο πεδίο ProxyAddresses](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) στην τοπική υπηρεσία καταλόγου Active Directory είναι μοναδική και η μορφή ταιριάζει sip:**Όνομα** χρήστη του χρήστη από το κέντρο διαχείρισης [Microsoft 365.](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)
- Εάν σκοπεύετε να διατηρήσετε μια ανάπτυξη του Skype για επιχειρήσεις Server και να έχετε χρήστες εσωτερικής εγκατάστασης και Online: ακολουθήστε την "Ρύθμιση υβριδικής λειτουργίας με το Teams και το **Skype για επιχειρήσεις Online"** στον Πίνακα Ελέγχου του Skype για επιχειρήσεις Server και μετακινήστε τους χρήστες online.
