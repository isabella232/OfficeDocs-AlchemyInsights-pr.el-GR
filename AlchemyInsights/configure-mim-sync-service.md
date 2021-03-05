---
title: Ρύθμιση παραμέτρων της υπηρεσίας συγχρονισμού MIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8472"
- "9004688"
ms.openlocfilehash: 48e9a0e8c26088b690092bfaedfba641841739f6
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481351"
---
# <a name="configure-mim-sync-service"></a>Ρύθμιση παραμέτρων της υπηρεσίας συγχρονισμού MIM

Η Υπηρεσία συγχρονισμού Microsoft Identity Manager (MIM) είναι ένα στοιχείο του MIM. Είναι μια κεντρική υπηρεσία εσωτερικής εγκατάστασης που αποθηκεύει και ενσωματώνει πληροφορίες για οργανισμούς που διαθέτουν πολλούς καταλόγους εσωτερικής εγκατάστασης και βάσεις δεδομένων. Ενδέχεται να μπορείτε να επιλύσετε το πρόβλημα με το MIM Sync, εάν το πρόβλημα έχει αντιμετωπιστεί σε μια πρόσφατη ενημέρωση του MIM ή είναι ένα από τα άλλα ζητήματα που αναφέρονται στην παρακάτω ενότητα.

**Προτεινόμενα βήματα**

1. Βεβαιωθείτε ότι χρησιμοποιείτε μια πρόσφατη ενημέρωση του MIM Sync και ελέγξτε τις σημειώσεις έκδοσης του [MIM Sync](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) για να προσδιορίσετε εάν το πρόβλημα έχει επιλυθεί σε μια ενημέρωση.
2. Εάν το πρόβλημα βρίσκεται στη γραμμή σύνδεσης "Generic LDAP", "Sql generic", "Lotus Domino" ή "Υπηρεσίες Web", βεβαιωθείτε ότι χρησιμοποιείτε μια πρόσφατη ενημέρωση των γενικών [γραμμών σύνδεσης.](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history)
3. Εάν η εκτέλεση MIM Sync σταματήσει να εμφανίζεται με σφάλμα, συμβουλευτείτε τον πίνακα εκτέλεσης κωδικών σφάλματος για [να](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) προσδιορίσετε τις πιθανές αιτίες.
4. Εάν η εκτέλεση σταματήσει με εξαίρεση **επέκταση-dll,** κάντε κλικ  σε αυτές τις λέξεις για να ανοίξετε το παράθυρο "Ιδιότητες αντικειμένου διαστήματος γραμμής σύνδεσης" και κάντε κλικ στην επιλογή "Ανίχνευση **στοίβας"** για να δείτε περισσότερες πληροφορίες σχετικά με την υποκείμενη αιτία, όπως περιγράφεται στο θέμα ["Επέκταση-DLL-Εξαίρεση".](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx)
5. Εάν το στοιχείο "Υπηρεσία ειδοποίησης αλλαγής κωδικού πρόσβασης" (PCNS) αναφέρει το σφάλμα **6025** στο αρχείο καταγραφής συμβάντων κατά το συγχρονισμό κωδικού πρόσβασης, ελέγξτε τον οδηγό για την αντιμετώπιση προβλημάτων με το σφάλμα [αναφοράς PCNS 6025.](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx)
6. Εάν ο πλήρης συγχρονισμός με τον παράγοντα  διαχείρισης υπηρεσιών FIM είναι αργός, ελέγξτε τη ρύθμιση αυτόματης ανάπτυξη για το TempDB, όπως περιγράφεται στην ενότητα "Αντιμετώπιση προβλημάτων αργού ή [προεξοχής πλήρους συγχρονισμού".](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx)
7. Εάν αντιμετωπίζετε ένα σφάλμα διακοπής του διακομιστή με αποτυχημένη δημιουργία-μέσω-web-services χρησιμοποιώντας τον Εκπρόσωπο διαχείρισης υπηρεσιών FIM, ανατρέξτε στις πληροφορίες [υποστήριξης: failed-creation-via-web-services για](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) μια επισκόπηση των αιτίων.

