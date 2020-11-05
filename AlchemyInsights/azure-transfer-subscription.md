---
title: Μεταφορά κυριότητας χρέωσης Azure
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
- "9003560"
- "6849"
ms.openlocfilehash: e9a1e74b321e2c2dda5f7a4f69681a0acf0635d5
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922075"
---
# <a name="transfer-azure-billing-ownership"></a>Μεταφορά κυριότητας χρέωσης Azure

Πραγματοποιήστε είσοδο στην [πύλη Azure](https://portal.azure.com/) ως διαχειριστής του λογαριασμού χρέωσης που έχει τη συνδρομή που θέλετε να μεταφέρετε. Εάν δεν είστε βέβαιοι εάν είστε και διαχειριστής ή εάν πρέπει να προσδιορίσετε ποιος είναι, ανατρέξτε στο θέμα [Καθορισμός διαχειριστή χρεώσεων λογαριασμού](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).

- Αναζητήστε τη **Διαχείριση κόστους + χρέωση**.
- Επιλέξτε **συνδρομές** από το αριστερό τμήμα παραθύρου. Ανάλογα με την Access, ίσως χρειαστεί να επιλέξετε ένα εύρος χρέωσης και, στη συνέχεια, **συνδρομές** ή **συνδρομές Azure**.
- Επιλέξτε **Μεταφορά κυριότητας χρέωσης** για τη συνδρομή που θέλετε να μεταφέρετε
- Πληκτρολογήστε τη διεύθυνση ηλεκτρονικού ταχυδρομείου ενός χρήστη που είναι διαχειριστής χρέωσης του λογαριασμού που θα είναι ο νέος κάτοχος για τη συνδρομή και, στη συνέχεια, επιλέξτε **Αποστολή αίτησης μεταφοράς**
- Ο χρήστης λαμβάνει ένα μήνυμα ηλεκτρονικού ταχυδρομείου με οδηγίες για την αναθεώρηση της αίτησής σας για μεταφορά. Για να εγκρίνει την αίτηση μεταφοράς, ο χρήστης επιλέγει τη σύνδεση στο μήνυμα ηλεκτρονικού ταχυδρομείου και ακολουθεί τις οδηγίες.

**Σημείωση** : Εάν μεταφέρετε την κυριότητα χρέωσης της συνδρομής σας σε ένα λογαριασμό χρήστη σε άλλο μισθωτή AD Azure, όλες οι αναθέσεις [ελέγχου πρόσβασης βάσει ρόλων (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)για τη διαχείριση πόρων στη συνδρομή καταργούνται οριστικά. Μόνο ο νέος κάτοχος θα έχει πρόσβαση για τη διαχείριση πόρων στη συνδρομή. Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα μεταφορά συνδρομής σε χρήστη σε άλλο ΜΙΣΘΩΤΉ AD Azure](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Προτεινόμενα έγγραφα**

- [Μεταφορά της κυριότητας χρέωσης μιας συνδρομής Azure σε άλλο λογαριασμό](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [Πληροφορίες σχετικά με τη μεταφορά της κυριότητας χρέωσης για μια συνδρομή Azure](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [Μεταφορά του Visual Studio, του δικτύου συνεργατών της Microsoft (MPN) και του Pay as you Go dev/Test συνδρομές](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Συνήθεις ερωτήσεις για την κυριότητα μεταφοράς](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Αντιμετώπιση προβλημάτων μεταβίβασης ιδιοκτησίας](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
