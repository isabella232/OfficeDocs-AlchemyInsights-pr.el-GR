---
title: Υποστηριζόμενοι τύποι συνδρομών
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
- "9003560"
- "6675"
ms.openlocfilehash: f11eabdc18f708e34a6a10c67bc3e7416330cbf34aec20209b42252ffa0ab018
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072160"
---
# <a name="supported-subscription-types"></a>Υποστηριζόμενοι τύποι συνδρομών

Εξετάστε τους υποστηριζόμενους τύπους συνδρομών για να προχωρήσετε περαιτέρω.

[Υποστηριζόμενοι τύποι συνδρομών](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**Μεταβίβαση κυριότητας χρεώσεων**

Πύλη Azure ως [διαχειριστής λογαριασμού](https://ms.portal.azure.com/) του λογαριασμού χρέωσης που έχει τη συνδρομή που θέλετε να μεταφέρετε

- Αναζητήστε τη **Διαχείριση κόστους + χρεώσεις**. Επιλέξτε **"Συνδρομές"** από το αριστερό τμήμα παραθύρου. Ανάλογα με την προσβασιμότητα, ίσως χρειαστεί να επιλέξετε ένα εύρος χρεώσεων και, στη συνέχεια, **Συνδρομές** ή **Συνδρομές Azure**.
- Επιλέξτε "Μεταφορά κυριότητας χρέωσης" για τη συνδρομή που θέλετε να μεταφέρετε
- Εισαγάγετε τη διεύθυνση ηλεκτρονικού ταχυδρομείου ενός χρήστη που είναι διαχειριστής χρέωσης του λογαριασμού που θα είναι ο νέος κάτοχος της συνδρομής και, στη συνέχεια, επιλέξτε **"Αποστολή αίτησης μεταφοράς"**
- Ο χρήστης λαμβάνει ένα μήνυμα ηλεκτρονικού ταχυδρομείου με οδηγίες για να εξετάσει την αίτηση μεταβίβασης. Για να εγκρίνετε την αίτηση μεταβίβασης, ο χρήστης επιλέγει τη σύνδεση στο μήνυμα ηλεκτρονικού ταχυδρομείου και ακολουθεί τις οδηγίες.

Σημείωση: Εάν μεταφέρετε την κυριότητα χρέωσης της συνδρομής σας στο λογαριασμό ενός χρήστη σε έναν άλλο μισθωτή Azure AD, όλες οι αναθέσεις ελέγχου πρόσβασης βάσει ρόλων [(RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) για τη διαχείριση πόρων στη συνδρομή καταργούνται οριστικά. Μόνο ο νέος κάτοχος θα έχει πρόσβαση στη διαχείριση πόρων της συνδρομής. Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα Μεταφορά συνδρομής σε χρήστη άλλου μισθωτή Azure AD.](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support)

**Μεταβίβαση κυριότητας συνδρομής**

Η δυνατότητα "Μεταφορά κυριότητας συνδρομής" προαπαιτούμενη πρόσβαση βάσει ρόλων (RBAC) για τη διαχείριση πόρων στη συνδρομή χάνει την πρόσβασή τους. Για περισσότερες πληροφορίες σχετικά με την προσθήκη μιας υπάρχουσας συνδρομής σε ένα μισθωτή, ανατρέξτε στο θέμα Συσχέτιση [ή προσθήκη συνδρομής Azure στο Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support)

- Η Μεταφορά συνδρομής με ένα υπάρχον ανεξόφλητο ποσό από τον τρέχοντα κύκλο χρέωσης δεν θα μεταφερθεί στο νέο μέσο πληρωμής του νέου λογαριασμού. Οι μόνες πληροφορίες που είναι διαθέσιμες στους χρήστες του νέου λογαριασμού είναι το κόστος του τελευταίου μήνα για τη συνδρομή σας. Το υπόλοιπο του ιστορικού χρήσης και χρέωσης δεν μεταφέρεται με τη συνδρομή.
- Η μεταβίβαση της κυριότητας Σύμβαση Enterprise συνδρομών (EA) υποστηρίζεται προς το παρόν μόνο στην Σύμβαση Enterprise πύλης
- Η μεταφορά μιας συνδρομής με πιστωτικό προσανατολισμό, όπως Visual Studio, BizSpark, Δίκτυο συνεργατών της Microsoft σε έναν νέο χρήστη απαιτεί να έχετε μια άδεια χρήσης δικτύου συνεργατών της Visual Studio/Microsoft για να αποδεχτείτε την αίτηση μεταφοράς
- Όλοι οι πόροι, όπως οι εικονικές μηχανές, οι δίσκοι και οι τοποθεσίες Web, μεταβιβάστε στον νέο λογαριασμό με επιτυχία. Οι ακόλουθοι πόροι μπορεί να επηρεαστούν σε μια μεταφορά συνδρομής μεταξύ μισθωτών:

**Υπηρεσίες τομέα Azure AD**

Θησαυροφυλάκια πλήκτρων Azure

- [SQL σχετικών χρηστών και βάσεων δεδομένων](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support) θα μπορούσε να επηρεάσει, ειδικά εάν ο πελάτης χρησιμοποιεί έναν Azure Active Directory έλεγχο ταυτότητας
- **Οι υπηρεσίες εφαρμογών** που έχουν ρυθμιστεί με Azure Active Directory ελέγχου ταυτότητας μπορεί να επηρεάσουν
- **Visual Studio ομάδας** Οι λογαριασμοί υπηρεσιών που είναι συνδεδεμένοι σε συνδρομές Azure ενδέχεται να χάσουν προσωρινά την πρόσβαση όταν ακυρωθεί η συνδεδεμένη συνδρομή Azure

**Προτεινόμενα έγγραφα**

Βήματα μετά την αποδοχή της κατοχής χρεώσεων:

- Για να διατηρήσετε την κατοχή χρεώσεων, αλλά να αλλάξετε τον τύπο της συνδρομής σας, ανατρέξτε στο εξής: [Αλλαγή της συνδρομής Azure σε άλλη προσφορά](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Μεταβίβαση των συνδρομών Visual Studio, του Δικτύου συνεργατών της Microsoft (MPN) και της "Ανάπτυξης/δοκιμής με πληρωμή ανάλογα με τη χρήση"](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Μεταβίβαση κυριότητας χρεώσεων Σύμβαση Enterprise συνδρομών (EA)](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [Συνήθεις ερωτήσεις για τη Μεταβίβαση κυριότητας](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Αντιμετώπιση προβλημάτων μεταβίβασης κυριότητας](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)