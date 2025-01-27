---
title: Σφάλματα εφαρμογών
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004342"
- "7841"
ms.openlocfilehash: ce4c89da79112726ed4fb25527edc8d082bd37f239595b9eab7279abeeecfd7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53931449"
---
# <a name="application-errors"></a>Σφάλματα εφαρμογών

Αναζητάτε πληροφορίες σχετικά με τους κωδικούς σφάλματος **AADSTS** που επιστρέφονται από την υπηρεσία διακριτικού ασφαλείας Azure Active Directory (Azure AD) (STS); Διαβάστε [τους κωδικούς σφαλμάτων ελέγχου ταυτότητας](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) και εξουσιοδότησης του Azure AD για να βρείτε περιγραφές σφαλμάτων AADSTS, επιδιορθώσεις και ορισμένες προτεινόμενες λύσεις.

Τα σφάλματα εξουσιοδότησης μπορεί να είναι αποτέλεσμα πολλών διαφορετικών προβλημάτων, τα περισσότερα από τα οποία προκαλούν σφάλμα 401 ή 403. Για παράδειγμα, όλα τα παρακάτω μπορεί να οδηγήσουν σε σφάλματα εξουσιοδότησης:

- Εσφαλμένες [ροές απόκτησης διακριτικού πρόσβασης](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) 
- Μη σωστά ρυθμισμένα [όρια δικαιωμάτων](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) 
- Έλλειψη [συναίνεσης](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

Για να επιλύσετε συνήθη σφάλματα εξουσιοδότησης, δοκιμάστε τα βήματα που παρέχονται παρακάτω που ταιριάζουν περισσότερο με το σφάλμα που λαμβάνετε. Ενδέχεται να ισχύουν περισσότερες από μία.

**Σφάλμα μη εξουσιοδότησης 401: Είναι έγκυρο το διακριτικό σας;**

Βεβαιωθείτε ότι η εφαρμογή σας παρουσιάζει ένα έγκυρο διακριτικό πρόσβασης στη Microsoft Graph ως μέρος της αίτησης. Αυτό το σφάλμα συχνά σημαίνει ότι το διακριτικό πρόσβασης ενδέχεται να λείπει στην κεφαλίδα της αίτησης ελέγχου ταυτότητας HTTP ή ότι το διακριτικό δεν είναι έγκυρο ή έχει λήξει. Συνιστάται ιδιαίτερα να χρησιμοποιήσετε τη Βιβλιοθήκη ελέγχου [ταυτότητας της Microsoft (MSAL) για](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) την απόκτηση διακριτικού πρόσβασης. Επιπλέον, αυτό το σφάλμα μπορεί να προκύψει εάν προσπαθήσετε να χρησιμοποιήσετε ένα διακριτικό πρόσβασης με ανάθεση που έχει παραχωρηθεί σε έναν προσωπικό λογαριασμό Microsoft για πρόσβαση σε ένα API που υποστηρίζει μόνο εταιρικούς ή σχολικούς λογαριασμούς (εταιρικούς λογαριασμούς).

**Σφάλμα απαγόρευσης 403: Έχετε επιλέξει το σωστό σύνολο δικαιωμάτων;**

Βεβαιωθείτε ότι έχετε ζητήσει το σωστό σύνολο δικαιωμάτων με βάση τα API της Microsoft Graph κλήσεις της εφαρμογής σας. Τα προτεινόμενα δικαιώματα με τα λιγότερο δικαιώματα παρέχονται σε όλα τα θέματα της μεθόδου Graph api της Microsoft. Επιπλέον, αυτά τα δικαιώματα πρέπει να εκχωρηθούν στην εφαρμογή από έναν χρήστη ή έναν διαχειριστή. Η εκχώρηση δικαιωμάτων συνήθως γίνεται μέσω μιας σελίδας συγκατάθεσης ή με εκχώρηση δικαιωμάτων χρησιμοποιώντας τη blade καταχώρησης της εφαρμογής πύλης Azure. Από τις **Ρυθμίσεις** για την εφαρμογή, κάντε κλικ στην επιλογή **Απαιτούμενα δικαιώματα** και, στη συνέχεια, κάντε κλικ στην επιλογή **Εκχώρηση δικαιωμάτων**.

- [Δικαιώματα του Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) 
- [Κατανόηση των δικαιωμάτων και της συναίνεσης στο Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

**Σφάλμα απαγόρευσης 403: Η εφαρμογή σας απέκτησε ένα διακριτικό ώστε να συμφωνεί με τα επιλεγμένα δικαιώματα;**

Βεβαιωθείτε ότι ο τύπος των δικαιωμάτων που ζητήθηκαν ή εκχωρήθηκαν συμφωνεί με τον τύπο διακριτικού πρόσβασης που αποκτά η εφαρμογή σας. Μπορεί να ζητάτε και να εκχωρείτε δικαιώματα εφαρμογής, αλλά να χρησιμοποιείτε διακριτικά ροής αλληλεπιδραστικού κώδικα με ανάθεση αντί για διακριτικά ροής διαπιστευτηρίων υπολογιστή-πελάτη ή να ζητάτε και να εκχωρείτε δικαιώματα ανάθεσης, αλλά να χρησιμοποιείτε διακριτικά ροής διαπιστευτηρίων προγράμματος-πελάτη αντί για διακριτικά ροής πληρεξούσιου κώδικα.

- [Αποκτήστε πρόσβαση εκ μέρους χρηστών και ανατεθειμένα δικαιώματα](https://docs.microsoft.com/graph/auth_v2_user) 
- [Azure AD v2.0 - Ροή κωδικών εξουσιοδότησης OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Αποκτήστε πρόσβαση χωρίς δικαιώματα χρήστη (υπηρεσία daemon) και εφαρμογής ](https://docs.microsoft.com/graph/auth_v2_service) 
- [Azure AD v2.0 - Ροή διαπιστευτηρίων προγράμματος-πελάτη OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

**Σφάλμα απαγόρευσης 403: Επαναφορά κωδικού πρόσβασης**

Προς το παρόν, δεν υπάρχουν δικαιώματα υπηρεσίας προς υπηρεσία daemon δικαιωμάτων εφαρμογής που επιτρέπουν την επαναφορά κωδικών πρόσβασης χρηστών. Αυτά τα API υποστηρίζονται μόνο χρησιμοποιώντας τις αλληλεπιδραστικές ανατεθειμένες ροές κωδικών με έναν συνδεδεμένο διαχειριστή.

- [Δικαιώματα του Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference)

**Σφάλμα απαγόρευσης 403: Έχει ο χρήστης πρόσβαση και άδεια χρήσης;**

Για ροές πληρεξούσιου κώδικα, το Microsoft Graph αξιολογεί εάν η αίτηση επιτρέπεται με βάση τα δικαιώματα που εκχωρούνται στην εφαρμογή και τα δικαιώματα που έχει ο συνδεδεμένος χρήστης. Γενικά, αυτό το σφάλμα υποδηλώνει ότι ο χρήστης δεν έχει αρκετά δικαιώματα για να εκτελέσει την αίτηση ή ο χρήστης δεν έχει άδεια χρήσης για τα δεδομένα στα οποία επιχειρεί να έχει πρόσβαση. Μόνο οι χρήστες με τα απαιτούμενα δικαιώματα ή άδειες χρήσης μπορούν να κάνουν την αίτηση με επιτυχία.

**Σφάλμα απαγόρευσης 403: Έχετε επιλέξει το σωστό API πόρου;**

Οι υπηρεσίες API, όπως το Microsoft Graph, ελέγχουν ότι η αξίωση aud (ακροατήριο) στο διακριτικό πρόσβασης που λαμβάνεται συμφωνεί με την τιμή που αναμένει για τον εαυτό της και, εάν όχι, αυτό έχει ως αποτέλεσμα ένα σφάλμα 403 Απαγορευμένο. Ένα συνηθισμένο λάθος που έχει ως αποτέλεσμα αυτό το σφάλμα είναι όταν προσπαθείτε να χρησιμοποιήσετε ένα διακριτικό που έχει αποκτηθεί για τα API του Azure AD Graph, τα API του Outlook ή τα API του SharePoint/OneDrive για να καλέσετε το Microsoft Graph (ή το αντίστροφο). Βεβαιωθείτε ότι ο πόρος (ή το εύρος) της εφαρμογής σας αποκτά ένα διακριτικό που να ταιριάζει με το API που καλεί η εφαρμογή.

**Λάθος αίτηση 400 ή Σφάλμα απαγόρευσης 403: Ο χρήστης συμμορφώνεται με τις πολιτικές πρόσβασης υπό όρους (CA) του οργανισμού του;**

Με βάση τις πολιτικές CA ενός οργανισμού, ένας χρήστης που αποκτά πρόσβαση σε πόρους του Microsoft Graph μέσω της εφαρμογής σας ενδέχεται να αμφισβητηθεί για πρόσθετες πληροφορίες που δεν υπάρχουν στο διακριτικό πρόσβασης που απέκτησε αρχικά η εφαρμογή σας. Σε αυτή την περίπτωση, η εφαρμογή σας λαμβάνει ένα 400 με σφάλμα *interaction_required* κατά την απόκτηση διακριτικού πρόσβασης ή ένα 403 με σφάλμα *insufficient_claims* κατά την κλήση στο Microsoft Graph. Και στις δύο περιπτώσεις, η απόκριση σφάλματος περιέχει πρόσθετες πληροφορίες που μπορούν να παρουσιάζονται στο τελικό σημείο εξουσιοδότησης για την πρόκληση του χρήστη για πρόσθετες πληροφορίες (όπως ο έλεγχος ταυτότητας πολλών παραγόντων ή η εγγραφή συσκευής).

- [Χειρισμός προκλήσεων πρόσβασης υπό όρους με χρήση του MSAL ](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [Οδηγίες για προγραμματιστές για πρόσβαση υπό όρους στο Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide)
