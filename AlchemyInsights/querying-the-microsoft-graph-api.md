---
title: Υποβολή ερωτημάτων στο API Graph Microsoft
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004345"
- "7846"
ms.openlocfilehash: eda5d8d1d76d0d87312b1441aeae89d8e250abe0e8b613d4a43fcc2345a6f021
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923239"
---
# <a name="querying-the-microsoft-graph-api"></a>Υποβολή ερωτημάτων στο API Graph Microsoft

Αυτό το θέμα μπορεί επίσης να ισχύει για προγραμματιστές που εξακολουθούν να χρησιμοποιούν το Azure AD Graph API. Ωστόσο, συνιστάται ιδιαίτερα **να χρησιμοποιείτε** το Microsoft Graph για όλα τα σενάρια διαχείρισης καταλόγου, ταυτότητας και πρόσβασης.

**Ζητήματα ελέγχου ταυτότητας ή εξουσιοδότησης**

- Εάν η  εφαρμογή σας δεν μπορεί να αποκτήσει διακριτικά για να καλέσει το Microsoft Graph, επιλέξτε "Πρόβλημα με τη λήψη διακριτικού πρόσβασης **(έλεγχος ταυτότητας)** της Microsoft Graph" για να λάβετε πιο συγκεκριμένη βοήθεια και υποστήριξη σχετικά με αυτό το θέμα.
- Εάν η εφαρμογή σας **λαμβάνει 401 ή 403** σφάλματα εξουσιοδότησης κατά την κλήση του Microsoft Graph, επιλέξτε την κατηγορία "Λήψη σφάλματος άρνησης πρόσβασης **(Εξουσιοδότηση)** API του Microsoft Graph" για να λάβετε πιο συγκεκριμένη βοήθεια και υποστήριξη σχετικά με αυτό το θέμα.

**Θέλω να χρησιμοποιήσω το Microsoft Graph, αλλά δεν είμαι βέβαιος από πού να ξεκινήσω**

Για να μάθετε περισσότερα σχετικά με το Microsoft Graph, ανατρέξτε στα θέμα:

- [Επισκόπηση του Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Επισκόπηση της διαχείρισης ταυτότητας και πρόσβασης στο Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Γρήγορα αποτελέσματα με τη δημιουργία εφαρμογών Graph Microsoft](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** - Δοκιμάστε τα API Graph Microsoft στον μισθωτή σας ή σε έναν μισθωτή επίδειξης

**Θέλω να χρησιμοποιήσω το Microsoft Graph, αλλά υποστηρίζει τα API καταλόγου v1.0 που χρειάζομαι;**

Το Microsoft Graph είναι το προτεινόμενο API για διαχείριση καταλόγου, ταυτότητας και πρόσβασης. Ωστόσο, εξακολουθούν να υπάρχουν ορισμένα κενά μεταξύ των πιθανών στο Azure AD Graph και του Microsoft Graph. Εξετάστε τα ακόλουθα άρθρα, τα οποία επισημαίνονται οι πιο ενημερωμένη διαφορές για να σας βοηθήσουν στην επιλογή σας:

- [Διαφορές τύπου πόρου μεταξύ του Azure AD Graph και του Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Διαφορές ιδιοτήτων μεταξύ του Azure AD Graph και του Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Διαφορές μεθόδου μεταξύ του Azure AD και του Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Όταν κάνω ερώτημα στο *αντικείμενο χρήστη,* λείπουν πολλές από τις ιδιότητές του**

`GET https://graph.microsoft.com/v1.0/users`Επιστρέφει μόνο 11 ιδιότητες, καθώς Graph Microsoft επιλέγει αυτόματα ένα προεπιλεγμένο σύνολο ιδιοτήτων χρήστη *για* να επιστρέψει. Εάν χρειάζεστε άλλες *ιδιότητες χρήστη,* χρησιμοποιήστε το $select για να επιλέξετε τις ιδιότητες που χρειάζεται η εφαρμογή σας. Δοκιμάστε το πρώτα **στην Εξερεύνηση Graph Microsoft.**

**Ορισμένες τιμές ιδιοτήτων χρήστη είναι *null, παρόλο* που γνωρίζω ότι έχουν οριστεί**

Η πιο πιθανή εξήγηση είναι ότι στην εφαρμογή είχε παραχωρηθεί το *δικαίωμα User.ReadBasic.All.* Αυτό επιτρέπει στην εφαρμογή να διαβάσει ένα περιορισμένο σύνολο ιδιοτήτων χρήστη, επιστρέφοντας όλες τις άλλες ιδιότητες ως null, ακόμα και αν έχουν οριστεί προηγουμένως. Δοκιμάστε να εκχωρήσετε το δικαίωμα *user.read.all της* εφαρμογής.

Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα Graph δικαιώματα χρήστη της Microsoft.](https://docs.microsoft.com/graph/permissions-reference#user-permissions)

**Έχω πρόβλημα με τη χρήση παραμέτρων ερωτήματος OData για το φιλτράρισμα δεδομένων στις αιτήσεις μου**

Παρόλο που το Microsoft Graph υποστηρίζει ένα ευρύ φάσμα παραμέτρων ερωτήματος OData, πολλές από αυτές τις παραμέτρους δεν υποστηρίζονται πλήρως από τις υπηρεσίες καταλόγου (πόρους που μεταβιβάζονται από *το directoryObject)* στο Microsoft Graph. Οι ίδιοι περιορισμοί που υπήρχαν στο Azure AD Graph διατηρούνται ως επί το μεγαλύτερο μέρος στο Microsoft Graph:

1. **Δεν υποστηρίζεται**: $count, $search και $filter τιμές *null* *ή όχι*
2. **Δεν υποστηρίζεται**: $filter σε ορισμένες ιδιότητες (ανατρέξτε στα θέματα πόρων για τις ιδιότητες με δυνατότητα φιλτραρίσματος)
3. **Δεν υποστηρίζεται:** σελιδοποίηση, φιλτράρισμα και ταξινόμηση ταυτόχρονα
4. **Δεν υποστηρίζεται:** φιλτράρισμα σε μια σχέση. Για παράδειγμα , βρείτε όλα τα μέλη της ομάδας μηχανικών που βρίσκονται στο Ηνωμένο Βασίλειο.
5. **Μερική υποστήριξη:**$orderby *χρήστη* (μόνο displayName και userPrincipalName) και *ομάδα*
6. **Μερική υποστήριξη**: $filter (υποστηρίζει μόνο *eq,* *startswith* ή *και* *,* και , και περιορίζεται *οποιαδήποτε)* υποστήριξη, το $expand (η ανάπτυξη των σχέσεων ενός αντικειμένου επιστρέφει όλες τις σχέσεις, αλλά η ανάπτυξη μιας συλλογής σχέσεων αντικειμένων είναι περιορισμένη)

Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Προσαρμογή απαντήσεων με παραμέτρους ερωτήματος.](https://docs.microsoft.com/graph/query-parameters)

**Το API που καλώ δεν λειτουργεί - πού μπορώ να κάνω περισσότερες δοκιμές;**

**Microsoft Graph Explorer** - Ελέγξτε τα API του Microsoft Graph στον μισθωτή σας ή  σε έναν μισθωτή επίδειξης και, επίσης, ελέγξτε τα δείγματα ερωτημάτων στην Εξερεύνηση Graph Microsoft.

**Όταν κάνω ερώτημα για δεδομένα, φαίνεται ότι έχω επιστρέψει ένα σύνολο μη ολοκληρωμένων δεδομένων**

Εάν υποβάλετε ερωτήματα σε μια συλλογή (όπως οι *χρήστες),* το Microsoft Graph χρησιμοποιεί όρια σελίδας από την πλευρά του διακομιστή, ώστε τα αποτελέσματα να επιστρέφονται πάντα με ένα προεπιλεγμένο μέγεθος σελίδας. Η εφαρμογή σας θα πρέπει πάντα να αναμένει ότι θα περιηφθεί σε συλλογές που επιστρέφονται από την υπηρεσία.

Για περισσότερες πληροφορίες, ανατρέξτε στα θέματα:

- [Βέλτιστες πρακτικές Graph Microsoft](https://docs.microsoft.com/graph/best-practices-concept)
- [Σελιδοποίηση δεδομένων Graph Microsoft στην εφαρμογή σας](https://docs.microsoft.com/graph/paging)

**Η εφαρμογή μου είναι πολύ αργή και επίσης επιβραδύνεται. Ποιες βελτιώσεις μπορώ να κάνω;**

Ανάλογα με το σενάριό σας, υπάρχουν διάφορες επιλογές στη διάθεσή σας για να κάνετε την εφαρμογή σας πιο αποτελεσματική και, σε ορισμένες περιπτώσεις, λιγότερο πιθανό να μετενεργιστείτε από την υπηρεσία (όταν πραγματοποιείτε πάρα πολλές κλήσεις).

Για να μάθετε περισσότερα, ανατρέξτε στα θέματα:

- [Βέλτιστες πρακτικές Graph Microsoft](https://docs.microsoft.com/graph/best-practices-concept)
- [Αιτήσεις δέσμης](https://docs.microsoft.com/graph/json-batching)
- [Παρακολούθηση αλλαγών μέσω ερωτήματος delta](https://docs.microsoft.com/graph/delta-query-overview)
- [Λήψη ειδοποίησης για αλλαγές μέσω webhook](https://docs.microsoft.com/graph/webhooks)
- [Οδηγίες για τον άμβλνο](https://docs.microsoft.com/graph/throttling)

**Πού μπορώ να βρω περισσότερες πληροφορίες σχετικά με σφάλματα και γνωστά προβλήματα;**

- [Πληροφορίες Graph απόκρισης σφάλματος της Microsoft](https://docs.microsoft.com/graph/errors)
- [Γνωστά προβλήματα με το Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**Πού μπορώ να ελέγξω την κατάσταση της διαθεσιμότητας υπηρεσίας και της συνδεσιμότητας;**

Η διαθεσιμότητα των υπηρεσιών και η συνδεσιμότητα των υποκείμενων υπηρεσιών στις οποίες μπορείτε να αποκτήσετε πρόσβαση μέσω του Microsoft Graph μπορεί να επηρεάσουν τη συνολική διαθεσιμότητα και τις επιδόσεις του Microsoft Graph.

- Για Azure Active Directory υπηρεσιών, ελέγξτε την κατάσταση των υπηρεσιών **Security + Identity** που παρατίθενται στη σελίδα κατάστασης [Azure.](https://azure.microsoft.com/status/)
- Για Office υπηρεσίες που συμβάλλουν στο Microsoft Graph, ελέγξτε την κατάσταση των υπηρεσιών που παρατίθενται [στον πίνακα εργαλείων Office υγείας υπηρεσιών.](https://portal.office.com/adminportal/home#/servicehealth)
