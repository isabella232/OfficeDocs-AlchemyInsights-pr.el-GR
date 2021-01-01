---
title: Μεταβίβαση κυριότητας χρεώσεων Azure
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
ms.openlocfilehash: 454ce626862bb4a2361abccd92ad0099b534388c
ms.sourcegitcommit: 059ad2936788266ea9714ec8c66d407d7261aeb6
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 12/29/2020
ms.locfileid: "49736878"
---
# <a name="transfer-azure-billing-ownership"></a>Μεταβίβαση κυριότητας χρεώσεων Azure

Πραγματοποιήστε είσοδο στην [πύλη Microsoft Azure](https://portal.azure.com/) ως διαχειριστής του λογαριασμού χρέωσης που έχει τη συνδρομή που θέλετε να μεταφέρετε. Εάν δεν είστε βέβαιος ότι είστε ο διαχειριστής του ή εάν πρέπει να προσδιορίσετε ποιος είναι, ανατρέξτε στο θέμα [ Καθορισμός διαχειριστή χρεώσεων λογαριασμού](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).

1. Αναζητήστε τη _Διαχείριση κόστους + χρεώσεις_.
1. Επιλέξτε **Συνδρομές** από το αριστερό τμήμα παραθύρου. Ανάλογα με την προσβασιμότητα, ίσως χρειαστεί να επιλέξετε ένα εύρος χρεώσεων και, στη συνέχεια, **Συνδρομές** ή **Συνδρομές Azure**.
1. Επιλέξτε **Μεταβίβαση κυριότητας χρέωσης** για τη συνδρομή που θέλετε να μεταφέρετε.
1. Πληκτρολογήστε τη διεύθυνση ηλεκτρονικού ταχυδρομείου ενός χρήστη που είναι διαχειριστής χρεώσεων του λογαριασμού που θα είναι ο νέος κάτοχος για τη συνδρομή και, στη συνέχεια, επιλέξτε **αποστολή αιτήματος μεταβίβασης**.
1. Ο χρήστης λαμβάνει ένα μήνυμα ηλεκτρονικού ταχυδρομείου με οδηγίες για να εξετάσει την αίτηση μεταβίβασης. Για να εγκρίνετε την αίτηση μεταβίβασης, ο χρήστης επιλέγει τη σύνδεση στο μήνυμα ηλεκτρονικού ταχυδρομείου και ακολουθεί τις οδηγίες.

Σημειώστε ότι εάν μεταφέρετε την κυριότητα της χρέωσης της συνδρομής σας στο λογαριασμό ενός χρήστη σε άλλο μισθωτή Microsoft Azure Active Directory, όλες οι αναθέσεις από τον [έλεγχο πρόσβασης βάσει ρόλων (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support), για τη διαχείριση πόρων στη συνδρομή καταργούνται οριστικά. Μόνο ο νέος κάτοχος θα έχει πρόσβαση στη διαχείριση πόρων της συνδρομής. Για περισσότερες πληροφορίες σχετικά με τον τρόπο με τον οποίο μπορείτε να αλλάξετε τον κατάλογο για μια συνδρομή, ανατρέξτε στο θέμα [Μεταβίβαση συνδρομής σε έναν χρήστη σε έναν άλλο μισθωτή του Microsoft Azure Active Directory](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

_**Σημαντική επίπτωση στα τιμολόγια σας**_: αν έχετε μεταβιβάσει την κυριότητα χρεώσεων για μια συνδρομή Azure, οι χρεώσεις σας θα πληρωθούν κατ' αναλογία. Θα έχετε τη δυνατότητα να αποκτήσετε πρόσβαση στα τιμολόγια σύμφωνα με τα εξής:  

1. Επιλέξτε τη συνδρομή σας από τη  [σελίδα Συνδρομές](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) στην πύλη Microsoft Azure ως [ένας χρήστης με πρόσβαση σε τιμολόγια](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)και, στη συνέχεια, επιλέξτε **Τιμολόγια**.
1. Κάντε κλικ στην επιλογή **Λήψη τιμολογίου** για να προβάλετε ένα αντίγραφο του τιμολογίου σε PDF. Εάν αναφέρει _Δεν είναι διαθέσιμο_, ανατρέξτε στο θέμα [Γιατί δεν βλέπω ένα τιμολόγιο για την τελευταία περίοδο χρέωσης;](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice).
1. Επίσης, μπορείτε να προβάλετε την καθημερινή χρήση σας κάνοντας κλικ στην **περίοδο χρέωσης** για να αποκτήσετε ένα PDF του τιμολογίου σας και ένα αντίγραφο του λεπτομερούς αρχείου καθημερινών χρήσεων (.CSV). Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Λήψη τιμολογίου και δεδομένων χρήσης](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support).

**Προτεινόμενα έγγραφα**

- [Μεταβίβαση κυριότητας χρέωσης μιας συνδρομής Azure σε άλλον λογαριασμό](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [Πληροφορίες σχετικά με τη Μεταβίβαση κυριότητας χρεώσεων για μια συνδρομή Azure](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [Μεταβίβαση των συνδρομών Visual Studio, του Δικτύου συνεργατών της Microsoft (MPN) και της "Ανάπτυξης/δοκιμής με πληρωμή ανάλογα με τη χρήση"](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Συνήθεις ερωτήσεις για τη Μεταβίβαση κυριότητας](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Αντιμετώπιση προβλημάτων μεταβίβασης κυριότητας](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
