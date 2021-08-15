---
title: Προβλήματα api Graph Microsoft
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
- "7759"
ms.openlocfilehash: 9df021211c8a65997889d9303dbf28a27104cfa95841d4cb810427c652ba0784
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975893"
---
# <a name="microsoft-graph-api-issues"></a>Προβλήματα api Graph Microsoft

Αυτό το θέμα μπορεί επίσης να ισχύει για προγραμματιστές που εξακολουθούν να χρησιμοποιούν το Azure AD Graph API. Ωστόσο, συνιστάται ιδιαίτερα **να χρησιμοποιείτε** το Microsoft Graph για όλα τα σενάρια διαχείρισης καταλόγου, ταυτότητας και πρόσβασης.

**Ζητήματα ελέγχου ταυτότητας ή εξουσιοδότησης**

- Εάν η  εφαρμογή σας δεν μπορεί να αποκτήσει διακριτικά για να καλέσει το Microsoft Graph, επιλέξτε "Πρόβλημα με τη λήψη διακριτικού πρόσβασης **(έλεγχος ταυτότητας)** της Microsoft Graph" για να λάβετε πιο συγκεκριμένη βοήθεια και υποστήριξη σχετικά με αυτό το θέμα.
- Εάν η εφαρμογή σας **λαμβάνει 401 ή 403** σφάλματα εξουσιοδότησης κατά την κλήση του Microsoft Graph, επιλέξτε την κατηγορία "Λήψη σφάλματος άρνησης πρόσβασης **(Εξουσιοδότηση)** API του Microsoft Graph" για να λάβετε πιο συγκεκριμένη βοήθεια και υποστήριξη σχετικά με αυτό το θέμα.

**Θέλω να χρησιμοποιήσω το Microsoft Graph, αλλά δεν είμαι βέβαιος από πού να ξεκινήσω**

- [Επισκόπηση του Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Επισκόπηση της διαχείρισης ταυτότητας και πρόσβασης στο Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Γρήγορα αποτελέσματα με τη δημιουργία εφαρμογών Graph Microsoft](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** - Δοκιμάστε τα API Graph Microsoft στον μισθωτή σας ή σε έναν μισθωτή επίδειξης

**Θέλω να χρησιμοποιήσω το Microsoft Graph, αλλά υποστηρίζει τα API καταλόγου v1.0 που χρειάζομαι;**

Το Microsoft Graph είναι το προτεινόμενο API για διαχείριση καταλόγου, ταυτότητας και πρόσβασης. Ωστόσο, εξακολουθούν να υπάρχουν ορισμένα κενά μεταξύ των πιθανών στο Azure AD Graph και του Microsoft Graph. Εξετάστε τα ακόλουθα άρθρα, τα οποία επισημαίνονται οι πιο ενημερωμένη διαφορές για να σας βοηθήσουν στην επιλογή σας:

- [Διαφορές τύπου πόρου μεταξύ του Azure AD Graph και του Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Διαφορές ιδιοτήτων μεταξύ του Azure AD Graph και του Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Διαφορές μεθόδου μεταξύ του Azure AD και του Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Το API που καλώ δεν λειτουργεί - πού μπορώ να κάνω περισσότερες δοκιμές;**

**Microsoft Graph Explorer** - Ελέγξτε τα API του Microsoft Graph στον μισθωτή σας ή  σε έναν μισθωτή επίδειξης και, επίσης, ελέγξτε τα δείγματα ερωτημάτων στην Εξερεύνηση Graph Microsoft.

**Η εφαρμογή μου είναι πολύ αργή και επίσης επιβραδύνεται. Ποιες βελτιώσεις μπορώ να κάνω;**

Ανάλογα με το σενάριό σας, υπάρχουν διάφορες επιλογές στη διάθεσή σας για να κάνετε την εφαρμογή σας πιο αποτελεσματική και, σε ορισμένες περιπτώσεις, λιγότερο πιθανό να μετενεργιστεί από την υπηρεσία (όταν πραγματοποιείτε πάρα πολλές κλήσεις).

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

Τα Graph εξουσιοδότησης της Microsoft μπορεί να είναι αποτέλεσμα πολλών διαφορετικών ζητημάτων, τα περισσότερα από τα οποία προκαλούν σφάλμα 401 ή 403. Για παράδειγμα, όλα τα παρακάτω μπορεί να οδηγήσουν σε σφάλματα εξουσιοδότησης:

- Εσφαλμένες [ροές απόκτησης διακριτικού πρόσβασης](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)
- Μη σωστά ρυθμισμένα [όρια δικαιωμάτων](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)
- Έλλειψη [συναίνεσης](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

***Λήξη υποστήριξης για τη Azure Active Directory ελέγχου ταυτότητας (ADAL) και το Azure AD Graph API (AAD Graph)***

**Από τις 30 Ιουνίου 2020,** δεν θα προσθέτουμε πλέον νέες δυνατότητες στο ADAL και το Azure AD Graph. Θα συνεχίσουμε να παρέχουμε ενημερώσεις τεχνικής υποστήριξης και ασφάλειας, αλλά δεν θα παρέχουμε πλέον ενημερώσεις δυνατοτήτων.

**Από τις 30 Ιουνίου 2022,** θα τερματίσουμε την υποστήριξη για το ADAL και το Azure AD Graph και δεν θα παρέχουμε πλέον τεχνική υποστήριξη ή ενημερώσεις ασφαλείας.

Οι εφαρμογές που χρησιμοποιούν ADAL σε υπάρχουσες εκδόσεις λειτουργικού συστήματος θα συνεχίσουν να λειτουργούν μετά από αυτό το χρονικό διάστημα, αλλά δεν θα λάβετε *τεχνική υποστήριξη ή ενημερώσεις ασφαλείας.*

Οι εφαρμογές που χρησιμοποιούν το Azure AD Graph μετά από αυτό το χρονικό διάστημα ενδέχεται να μην λαμβάνουν πλέον απαντήσεις από το τελικό Graph Azure AD.

**Μετεγκατάσταση ADAL**

Συνιστάται να κάνετε ενημέρωση στη [Βιβλιοθήκη ελέγχου ταυτότητας της Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), η οποία διαθέτει τις πιο πρόσφατες δυνατότητες και ενημερώσεις ασφαλείας.

Εάν χρησιμοποιείτε εφαρμογές της Microsoft, να γνωρίζετε ότι η Microsoft βρίσκεται σε διαδικασία μετεγκατάστασης των εφαρμογών της στο MSAL μέχρι το τέλος της προθεσμίας υποστήριξης, εξασφαλίζοντας ότι θα επωφεληθούν από τις συνεχείς βελτιώσεις ασφάλειας και δυνατοτήτων της MSAL.

1. [Διαβάστε τις Συνήθεις ερωτήσεις του ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Μάθετε πώς μπορείτε να μετεγκαταστήσετε εφαρμογές ανά πλατφόρμα](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Εάν χρειάζεστε βοήθεια για να κατανοήσετε ποιες από τις εφαρμογές σας χρησιμοποιούν το ADAL, συνιστάται να εξετάσετε τον πηγαίο κώδικα όλων των εφαρμογών σας και, εάν υπάρχει, να χρησιμοποιήσετε τυχόν ISV ή υπηρεσίες παροχής εφαρμογών. Η υποστήριξη της Microsoft μπορεί επίσης να σας παράσχει μια λίστα με όλες τις εφαρμογές ADAL που δεν είναι της Microsoft στον μισθωτή σας.

**Μετεγκατάσταση του AAD Graph**

Για εφαρμογές που χρησιμοποιούν το Azure AD Graph, ακολουθήστε τις οδηγίες μας για τη μετεγκατάσταση εφαρμογών [Azure AD Graph στο Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [Η λίστα ελέγχου μετεγκατάστασης παρέχει ένα σημείο εκκίνησης](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).
2. Η πύλη καταχώρησης εφαρμογών Azure δείχνει ποιες εφαρμογές χρησιμοποιούν το AAD Graph. Συνιστάται να εξετάσετε ολόκληρο τον πηγαίο κώδικα των εφαρμογών σας και, εάν ισχύει, επικοινωνήστε με οποιονδήποτε ISV ή πάροχο εφαρμογών. Η υποστήριξη της Microsoft μπορεί επίσης να σας παρέχει μια λίστα όλων των Graph AAD στο μισθωτή σας.
3. Για να έχει πρόσβαση η εφαρμογή σας σε δεδομένα στο Microsoft Graph, ο χρήστης ή ο διαχειριστής πρέπει να της εκχωρήσει τα σωστά δικαιώματα μέσω μιας διαδικασίας συγκατάθεσης. Η [αναφορά δικαιωμάτων Graph](https://docs.microsoft.com/graph/permissions-reference) Microsoft παραθέτει τα δικαιώματα που σχετίζονται με κάθε κύριο σύνολο API Graph Microsoft. Παρέχει επίσης οδηγίες σχετικά με τον τρόπο χρήσης των δικαιωμάτων.
