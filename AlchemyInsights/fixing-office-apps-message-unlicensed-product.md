---
title: Δεν είναι δυνατή η ενεργοποίηση του Office
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
- "2000023"
- "3509"
ms.openlocfilehash: 9a33b7880aff6016ef6df88960d6f59ac9dd50382c7e99d72ca36bc3c9f344ea
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53928369"
---
# <a name="unable-to-activate-office"></a>Δεν είναι δυνατή η ενεργοποίηση του Office

**Σημείωση:** Εάν χρησιμοποιείτε μια παλαιότερη έκδοση του Windows (Για παράδειγμα, Windows 7), βεβαιωθείτε ότι το TLS 1.2 είναι ενεργοποιημένο ως προεπιλογή. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα Ενημέρωση για την ενεργοποίηση [των TLS 1.1 και TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)ως προεπιλεγμένων ασφαλών πρωτοκόλλων στο WinHTTP στο Windows.

- Ελέγξτε εάν έχει λήξει η κατάσταση της συνδρομής σας.
- Βεβαιωθείτε ότι έχετε μια συνδρομή που επιτρέπει άδειες χρήσης προγράμματος-πελάτη, όπως το Office 365 για Επιχειρήσεις ή το Office 365 Premium για Επιχειρήσεις και [βεβαιωθείτε ότι έχει εκχωρηθεί άδεια στον χρήστη](/microsoft-365/admin/manage/assign-licenses-to-users).
- Βεβαιωθείτε ότι ο χρήστης πραγματοποιεί είσοδο στο Office με τον ίδιο λογαριασμό στον οποίο έχει εκχωρηθεί η άδεια χρήσης.
- Επισκεφθείτε τη [σελίδα εύρυθμης λειτουργίας των υπηρεσιών του Office 365](/office365/enterprise/view-service-health) για να δείτε αν υπάρχουν γνωστά προβλήματα με την υπηρεσία.
- Ελέγξτε το τείχος προστασίας, το λογισμικό προστασίας από ιούς και τις ρυθμίσεις διακομιστή μεσολάβησης για να επιβεβαιώσετε ότι δεν εμποδίζουν την πρόσβαση στο Internet στις εφαρμογές του Microsoft 365. Ανατρέξτε στο θέμα [Διευθύνσεις URL και εύρη διευθύνσεων IP του Office 365](/office365/enterprise/urls-and-ip-address-ranges "Διευθύνσεις URL και εύρη διευθύνσεων IP του Office 365").

**Συμβουλή** Σε υπολογιστές με Windows, μπορούμε να διαγνώσουμε και να διορθώσουμε αυτόματα αρκετά κοινά προβλήματα εισόδου του Office για εσάς. Κατεβάστε και εκτελέστε τον **[Βοηθό υποστήριξης και αποκατάστασης για το Office 365](https://aka.ms/SaRA-OfficeSignInScenario)** για να χρησιμοποιήσετε το αυτοματοποιημένο εργαλείο μας.

Χρησιμοποιήστε τις παρακάτω ενέργειες αντιμετώπισης προβλημάτων:

- Ανοίξτε μια εφαρμογή του Office και [Αποσυνδεθείτε](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) από όλους τους υπάρχοντες λογαριασμούς χρηστών. [Κατάργηση](/microsoft-365/admin/manage/remove-licenses-from-users) και [εκ νέου ανάθεση](/microsoft-365/admin/manage/assign-licenses-to-users)της άδεια χρήσης του Office και, στη συνέχεια, [συνδεθείτε στο Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) χρησιμοποιώντας το λογαριασμό χρήστη που επηρεάζεται.
- Εκτέλεση του προγράμματος [Αντιμετώπιση προβλημάτων ενεργοποίησης](https://aka.ms/SARA-OfficeActivation-Alchemy)
- [Επαναφορά κατάστασης ενεργοποίησης του Office](/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Επαναφορά κατάστασης ενεργοποίησης του Office")
- [Πραγματοποίηση επιδιόρθωσης του Office μέσω Internet](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

Για πρόσθετες λύσεις αντιμετώπισης προβλημάτων, ανατρέξτε στα θέματα:  

- [Σφάλματα "Προϊόν χωρίς άδεια χρήσης" και σφάλματα ενεργοποίησης στο Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- ["Λυπούμαστε, δεν είναι δυνατή η σύνδεση στο λογαριασμό σας. Σφάλμα "Δοκιμάστε ξανά αργότερα" κατά την ενεργοποίηση του Office](/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)