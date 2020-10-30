---
title: Υποστηριζόμενοι τύποι συνδρομής
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
- "6675"
ms.openlocfilehash: 46bc60435c3f8477e9f274d90c39d0f1c6a523c6
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807562"
---
# <a name="supported-subscription-types"></a>Υποστηριζόμενοι τύποι συνδρομής

Παρακαλούμε εξετάστε τους υποστηριζόμενους τύπους συνδρομής για να προχωρήσετε περαιτέρω.

[Υποστηριζόμενοι τύποι συνδρομής](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**Μεταβίβαση κυριότητας χρέωσης**

Πύλη Azure ως [διαχειριστής λογαριασμού](https://ms.portal.azure.com/) του λογαριασμού χρέωσης που έχει τη συνδρομή που θέλετε να μεταφέρετε

- Αναζητήστε τη **Διαχείριση κόστους + χρέωση** . Επιλέξτε **συνδρομές** από το αριστερό τμήμα παραθύρου. Ανάλογα με την Access, ίσως χρειαστεί να επιλέξετε ένα εύρος χρέωσης και, στη συνέχεια, **συνδρομές** ή **συνδρομές Azure** .
- Επιλέξτε Μεταφορά κυριότητας χρέωσης για τη συνδρομή που θέλετε να μεταφέρετε
- Πληκτρολογήστε τη διεύθυνση ηλεκτρονικού ταχυδρομείου ενός χρήστη που είναι διαχειριστής χρέωσης του λογαριασμού που θα είναι ο νέος κάτοχος για τη συνδρομή και, στη συνέχεια, επιλέξτε **Αποστολή αίτησης μεταφοράς**
- Ο χρήστης λαμβάνει ένα μήνυμα ηλεκτρονικού ταχυδρομείου με οδηγίες για την αναθεώρηση της αίτησής σας για μεταφορά. Για να εγκρίνει την αίτηση μεταφοράς, ο χρήστης επιλέγει τη σύνδεση στο μήνυμα ηλεκτρονικού ταχυδρομείου και ακολουθεί τις οδηγίες.

Σημείωση: Εάν μεταφέρετε την κυριότητα χρέωσης της συνδρομής σας σε ένα λογαριασμό χρήστη σε άλλο μισθωτή AD Azure, όλες οι αναθέσεις [ελέγχου πρόσβασης βάσει ρόλων (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) για τη διαχείριση πόρων στη συνδρομή καταργούνται οριστικά. Μόνο ο νέος κάτοχος θα έχει πρόσβαση για τη διαχείριση πόρων στη συνδρομή. Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα μεταφορά συνδρομής σε χρήστη σε άλλο ΜΙΣΘΩΤΉ AD Azure](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Μεταβίβαση κυριότητας της συνδρομής**

Προϋποθέσεις μεταβίβασης της κυριότητας συνδρομής ο ρόλος που βασίζεται στην Access (RBAC) για τη διαχείριση πόρων στη συνδρομή χάνει την πρόσβασή τους. Για περισσότερες πληροφορίες σχετικά με την προσθήκη μιας υπάρχουσας συνδρομής σε έναν μισθωτή, ανατρέξτε στο θέμα [συσχέτιση ή προσθήκη μιας συνδρομής Azure στην υπηρεσία καταλόγου Active Directory Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

- Η μεταφορά συνδρομής με ένα υπάρχον εκκρεμές ποσό από τον τρέχοντα κύκλο χρέωσης δεν θα μεταφερθεί στο νέο μέσο πληρωμής στον νέο λογαριασμό. Οι μόνες πληροφορίες που είναι διαθέσιμες στους χρήστες στο νέο λογαριασμό είναι το κόστος του τελευταίου μήνα για τη συνδρομή σας. Το υπόλοιπο του ιστορικού χρήσης και χρεώσεων δεν μεταβιβάζεται με τη συνδρομή.
- Η μεταβίβαση χρεώσεων για τις συνδρομές εταιρικών συμφωνητικών (EA) υποστηρίζεται αυτή τη στιγμή στην πύλη εταιρικών συμφωνητικών μόνο
- Η μεταφορά μιας συνδρομής με δυνατότητα πίστωσης, όπως το Visual Studio, το BizSpark, το δίκτυο συνεργατών της Microsoft σε έναν νέο χρήστη απαιτεί να έχετε μια άδεια χρήσης του δικτύου συνεργατών του Visual Studio/Microsoft για να αποδεχθείτε την αίτηση μεταφοράς
- Όλοι οι πόροι, όπως οι εικονικές μηχανές, οι δίσκοι και οι τοποθεσίες Web, μεταφέρουν με επιτυχία τον νέο λογαριασμό. Οι ακόλουθοι πόροι μπορεί να επηρεαστούν σε μια μεταφορά συνδρομής μεταξύ μισθωτών:

**Υπηρεσίες τομέα AD Azure**

Θόλοι κλειδιών Azure

- [Οι συσχετισμένοι χρήστες και βάσεις δεδομένων SQL](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support) μπορεί να επηρεαστούν, ειδικά εάν ο πελάτης χρησιμοποιεί έναν έλεγχο ταυτότητας που σχετίζεται με το Azure Active Directory
- Οι **υπηρεσίες εφαρμογών** που έχουν ρυθμιστεί με τον έλεγχο ταυτότητας του Azure Active Directory μπορεί να επηρεαστούν
- **Ομάδα του Visual Studio** Οι λογαριασμοί υπηρεσιών που είναι συνδεδεμένοι σε συνδρομές Azure ενδέχεται να χάσουν προσωρινά την πρόσβαση όταν ακυρωθεί η συνδεδεμένη συνδρομή Azure

**Προτεινόμενα έγγραφα**

Βήματα μετά την αποδοχή της κυριότητας χρέωσης:

- Για να διατηρήσετε την κυριότητα των χρεώσεων, αλλά να αλλάξετε τον τύπο της συνδρομής σας, ανατρέξτε στο θέμα: [Αλλαγή της συνδρομής σας Azure σε άλλη προσφορά](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Μεταφορά του Visual Studio, του δικτύου συνεργατών της Microsoft (MPN) και του Pay as you Go dev/Test συνδρομές](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Μεταβίβαση της κυριότητας χρεώσεων για συνδρομές εταιρικών συμφωνητικών (EA)](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [Συνήθεις ερωτήσεις για την κυριότητα μεταφοράς](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Αντιμετώπιση προβλημάτων μεταβίβασης ιδιοκτησίας](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)