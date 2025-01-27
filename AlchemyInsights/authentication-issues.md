---
title: Προβλήματα ελέγχου ταυτότητας
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7748"
- "9004339"
ms.openlocfilehash: c7e6d96940f8d7052ee4b49b22c0d1d7d5bd5f9277f4a7eff709def1da2e13af
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54019508"
---
# <a name="authentication-issues"></a>Προβλήματα ελέγχου ταυτότητας

**Αναζητάτε πληροφορίες σχετικά με τους κωδικούς σφάλματος AADSTS που επιστρέφονται από την υπηρεσία διακριτικών ασφαλείας (STS) του Azure Active Directory (Azure AD);** Ανατρέξτε στο θέμα[Έλεγχος ταυτότητας και εξουσιοδότηση του Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) για να βρείτε περιγραφές των σφαλμάτων AADSTS, επιδιορθώσεις και ορισμένες προτεινόμενες λύσεις.

Τα σφάλματα εξουσιοδότησης μπορεί να είναι αποτέλεσμα πολλών διαφορετικών προβλημάτων, τα περισσότερα από τα οποία προκαλούν σφάλμα 401 ή 403. Για παράδειγμα, τα παρακάτω προβλήματα μπορούν όλα να οδηγήσουν σε σφάλματα εξουσιοδότησης:

- Εσφαλμένες [ροές απόκτησης διακριτικού πρόσβασης](https://docs.microsoft.com/azure/active-directory/develop/authentication-vs-authorization) 
- Μη σωστά ρυθμισμένα [όρια δικαιωμάτων](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 
- Έλλειψη [συναίνεσης](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant#understanding-user-and-admin-consent)

Για την επίλυση συνηθισμένων σφαλμάτων εξουσιοδότησης, δοκιμάστε τα βήματα που παρέχονται παρακάτω τα οποία ταιριάζουν περισσότερο με το σφάλμα που λαμβάνετε. Ενδέχεται να ισχύουν περισσότερα από ένα βήματα για ένα σφάλμα που λαμβάνετε.

**Σφάλμα μη εξουσιοδότησης 401: Είναι έγκυρο το διακριτικό σας;**

Βεβαιωθείτε ότι η εφαρμογή σας παρουσιάζει ένα έγκυρο διακριτικό πρόσβασης στο Microsoft Graph ως μέρος της αίτησης. Αυτό το σφάλμα συχνά σημαίνει ότι το διακριτικό πρόσβασης ενδέχεται να λείπει στην κεφαλίδα της αίτησης ελέγχου ταυτότητας HTTP ή ότι το διακριτικό δεν είναι έγκυρο ή έχει λήξει. Συνιστάται ιδιαίτερα να χρησιμοποιείτε τη Βιβλιοθήκη ελέγχου ταυτότητας της Microsoft (MSAL) για την απόκτηση διακριτικού πρόσβασης. Επιπλέον, αυτό το σφάλμα ενδέχεται να προκύψει εάν προσπαθήσετε να χρησιμοποιήσετε ένα ανατεθειμένο διακριτικό πρόσβασης που έχει παραχωρηθεί σε έναν προσωπικό λογαριασμό Microsoft για πρόσβαση σε API που υποστηρίζει μόνο επαγγελματικούς ή σχολικούς λογαριασμούς (εταιρικούς λογαριασμούς).

**Σφάλμα απαγόρευσης 403: Έχετε επιλέξει το σωστό σύνολο δικαιωμάτων;**

Βεβαιωθείτε ότι έχετε ζητήσει το σωστό σύνολο δικαιωμάτων με βάση τα API του Microsoft Graph για τις κλήσεις εφαρμογής. Τα προτεινόμενα δικαιώματα ελάχιστου επιπέδου παρέχονται σε όλα τα θέματα μεθόδου αναφοράς API του Microsoft Graph. Επιπλέον, αυτά τα δικαιώματα πρέπει να εκχωρηθούν στην εφαρμογή από έναν χρήστη ή έναν διαχειριστή. Η εκχώρηση δικαιωμάτων συνήθως συμβαίνει μέσω μιας σελίδας δικαιωμάτων ή της χρήσης της εγγραφής εφαρμογής της πύλης Microsoft Azure. Από τις **Ρυθμίσεις** για την εφαρμογή, κάντε κλικ στην επιλογή **Απαιτούμενα δικαιώματα** και, στη συνέχεια, κάντε κλικ στην επιλογή **Εκχώρηση δικαιωμάτων**. Για περισσότερες πληροφορίες, ανατρέξτε στα θέματα:

- [Δικαιώματα του Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) 
- [Κατανόηση των δικαιωμάτων και της συναίνεσης στο Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)

**Σφάλμα απαγόρευσης 403: Η εφαρμογή σας απέκτησε ένα διακριτικό ώστε να συμφωνεί με τα επιλεγμένα δικαιώματα;**

Βεβαιωθείτε ότι οι τύποι δικαιωμάτων που ζητήθηκαν ή εκχωρήθηκαν συμφωνούν με τον τύπο του διακριτικού πρόσβασης που αποκτά η εφαρμογή σας. Μπορεί να ζητάτε και να εκχωρείτε δικαιώματα εφαρμογής, αλλά να χρησιμοποιείτε ανατεθειμένα αλληλεπιδραστικά διακριτικά ροής κώδικα αντί για διακριτικά ροής διαπιστευτηρίων προγράμματος-πελάτη ή να ζητάτε και να εκχωρείτε ανατεθειμένα δικαιώματα, αλλά χρησιμοποιώντας διακριτικά ροής διαπιστευτηρίων προγράμματος-πελάτη αντί για ανατεθειμένα διακριτικά ροής κώδικα.

Για περισσότερες πληροφορίες σχετικά με τη λήψη διακριτικών, ανατρέξτε στα θέματα:

- [Αποκτήστε πρόσβαση εκ μέρους χρηστών και ανατεθειμένα δικαιώματα](https://docs.microsoft.com/graph/auth-v2-user) 
- [Azure AD v2.0 - Ροή κωδικών εξουσιοδότησης OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Αποκτήστε πρόσβαση χωρίς δικαιώματα χρήστη (υπηρεσία daemon) και εφαρμογής ](https://docs.microsoft.com/graph/auth-v2-service) 
- [Azure AD v2.0 - Ροή διαπιστευτηρίων προγράμματος-πελάτη OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

**Σφάλμα απαγόρευσης 403: Επαναφορά κωδικού πρόσβασης**

Προς το παρόν, δεν υπάρχουν δικαιώματα υπηρεσίας προς υπηρεσία daemon δικαιωμάτων εφαρμογής που επιτρέπουν την επαναφορά κωδικών πρόσβασης χρηστών. Αυτά τα API υποστηρίζονται μόνο χρησιμοποιώντας τις αλληλεπιδραστικές ανατεθειμένες ροές κωδικών με έναν συνδεδεμένο διαχειριστή. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Δικαιώματα του Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference).

**Σφάλμα απαγόρευσης 403: Έχει ο χρήστης πρόσβαση και άδεια χρήσης;**

Για ροές κωδικών με ανάθεση, το Microsoft Graph αξιολογεί εάν η αίτηση έχει επιτραπεί με βάση τα δικαιώματα που έχουν παραχωρηθεί στην εφαρμογή και τα δικαιώματα που έχει ο συνδεδεμένος χρήστης. Γενικά, αυτό το σφάλμα υποδηλώνει ότι ο χρήστης δεν έχει αρκετά δικαιώματα για να εκτελέσει την αίτηση **ή** ο χρήστης δεν έχει άδεια χρήσης για τα δεδομένα στα οποία επιχειρεί να έχει πρόσβαση. Μόνο οι χρήστες με τα απαιτούμενα δικαιώματα ή άδειες χρήσης μπορούν να κάνουν την αίτηση με επιτυχία.

**Σφάλμα απαγόρευσης 403: Έχετε επιλέξει το σωστό API πόρου;**

Οι υπηρεσίες API όπως το Microsoft Graph ελέγχουν αν η αίτηση *aud* (ακροατήριο) στο ληφθέν διακριτικό πρόσβασης συμφωνεί με την τιμή που αναμένει για την ίδια και, εάν όχι, προκύπτει Σφάλμα απαγόρευσης 403. Ένα συνηθισμένο λάθος που έχει ως αποτέλεσμα αυτό το σφάλμα είναι όταν προσπαθείτε να χρησιμοποιήσετε ένα διακριτικό που έχει αποκτηθεί για τα API του Azure AD Graph, τα API του Outlook ή τα API του SharePoint/OneDrive για να καλέσετε το Microsoft Graph (ή το αντίστροφο). Βεβαιωθείτε ότι ο πόρος (ή το εύρος) της εφαρμογής σας αποκτά ένα διακριτικό που να ταιριάζει με το API που καλεί η εφαρμογή.

**Λάθος αίτηση 400 ή Σφάλμα απαγόρευσης 403: Ο χρήστης συμμορφώνεται με τις πολιτικές πρόσβασης υπό όρους (CA) του οργανισμού του;**

Με βάση τις πολιτικές πρόσβασης υπό όρους (CA) ενός οργανισμού, ένας χρήστης που έχει πρόσβαση στους πόρους του Microsoft Graph μέσω της εφαρμογής σας μπορεί να αντιμετωπίσει δυσκολίες για πρόσθετες πληροφορίες που δεν υπάρχουν στο διακριτικό πρόσβασης που απέκτησε αρχικά η εφαρμογή σας. Σε αυτή την περίπτωση, η εφαρμογή σας λαμβάνει ένα **400 με σφάλμα *interaction_required*** κατά την απόκτηση διακριτικού πρόσβασης ή ένα **403 με σφάλμα *insufficient_claims*** κατά την κλήση στο Microsoft Graph. Και στις δύο περιπτώσεις, η απάντηση σφάλματος περιέχει πρόσθετες πληροφορίες που μπορούν να παρουσιαστούν στο εξουσιοδοτημένο τελικό σημείο για να ζητήσει από τον χρήστη πρόσθετες πληροφορίες (όπως έλεγχο ταυτότητας πολλών παραγόντων ή εγγραφή συσκευής).

Για περισσότερες πληροφορίες σχετικά με την πρόσβαση υπό όρους, ανατρέξτε στα θέματα:

- [Χειρισμός των πρόκλησης πρόσβασης υπό όρους με χρήση του MSAL](https://docs.microsoft.com/azure/active-directory/develop/msal-error-handling-dotnet#conditional-access-and-claims-challenges) 
- [Οδηγίες για προγραμματιστές για πρόσβαση υπό όρους στο Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/v2-conditional-access-dev-guide)

***Λήξη υποστήριξης για τη Azure Active Directory ελέγχου ταυτότητας (ADAL) και το Azure AD Graph API (AAD Graph)***

- Από τις 30 Ιουνίου 2020, δεν θα προσθέσουμε άλλες νέες δυνατότητες στη Βιβλιοθήκη ελέγχου ταυτότητας του Azure Active Directory (ADAL) και του Azure AD Graph API (AAD Graph). Θα συνεχίσουμε να παρέχουμε ενημερώσεις τεχνικής υποστήριξης και ασφάλειας, αλλά δεν θα παρέχουμε πλέον ενημερώσεις δυνατοτήτων.
- Από τις 30 Ιουνίου 2022, θα τερματίσουμε την υποστήριξη για το ADAL και το AAD Graph και δεν θα παρέχουμε πλέον τεχνική υποστήριξη ή ενημερώσεις ασφαλείας.
    - Οι εφαρμογές που χρησιμοποιούν το ADAL σε υπάρχουσες εκδόσεις λειτουργικού συστήματος θα συνεχίσουν να λειτουργούν μετά από αυτό το χρονικό διάστημα, αλλά δεν θα λαμβάνουν καμία τεχνική υποστήριξη ή ενημερώσεις ασφαλείας.
    - Οι εφαρμογές που θα χρησιμοποιούν το AAD Graph μετά από αυτό το χρονικό διάστημα ενδέχεται να μην λαμβάνουν πλέον απαντήσεις από το τελικό σημείο του AAD Graph.

**Μετεγκατάσταση ADAL**

Συνιστάται να κάνετε ενημέρωση στη [Βιβλιοθήκη ελέγχου ταυτότητας της Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), η οποία διαθέτει τις πιο πρόσφατες δυνατότητες και ενημερώσεις ασφαλείας. Αυτή η ενέργεια είναι στο πλαίσιο της μετεγκατάστασης των εφαρμογών της Microsoft στο MSAL μέχρι την προθεσμία λήξης της υποστήριξης. Ο στόχος της μετεγκατάστασης των εφαρμογών της Microsoft στο MSAL είναι να εξασφαλιστεί ότι οι εφαρμογές επωφελούνται από τις συνεχείς βελτιώσεις ασφάλειας και δυνατοτήτων του MSAL.

- [Διαβάστε τις Συνήθεις ερωτήσεις του ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- [Μάθετε πώς μπορείτε να μετεγκαταστήσετε εφαρμογές ανά πλατφόρμα](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- Εάν χρειάζεστε βοήθεια για να κατανοήσετε ποιες από τις εφαρμογές σας χρησιμοποιούν το ADAL, συνιστάται να εξετάσετε τον πηγαίο κώδικα όλων των εφαρμογών σας και, εάν ισχύει, να προσεγγίσετε οποιονδήποτε ανεξάρτητο προμηθευτή λογισμικού (ISV) ή υπηρεσίες παροχής εφαρμογών. Η υποστήριξη της Microsoft μπορεί επίσης να σας παράσχει μια λίστα με όλες τις εφαρμογές ADAL που δεν είναι της Microsoft στον μισθωτή σας.

**Μετεγκατάσταση του AAD Graph**

Για τις εφαρμογές που χρησιμοποιούν το AAD Graph, ακολουθήστε τις οδηγίες μας για [μετεγκατάσταση των εφαρμογών του Azure AD Graph στο Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist?view=graph-rest-1.0&preserve-view=true).

- [Η λίστα ελέγχου μετεγκατάστασης παρέχει ένα σημείο εκκίνησης](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
- Η πύλη καταχώρησης εφαρμογών Azure δείχνει ποιες εφαρμογές χρησιμοποιούν το AAD Graph. Συνιστάται να εξετάσετε ολόκληρο τον πηγαίο κώδικα των εφαρμογών σας και, εάν ισχύει, επικοινωνήστε με οποιονδήποτε ISV ή πάροχο εφαρμογών. Η υποστήριξη της Microsoft μπορεί επίσης να σας παράσχει τις πληροφορίες για όλη τη χρήση του AAD Graph στον μισθωτή σας.

 










