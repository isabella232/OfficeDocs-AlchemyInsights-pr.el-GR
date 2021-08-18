---
title: Ζητήματα με συνδέσεις και διευθύνσεις URL
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: d85069970fe6bc6cc7a8488c49c0e6236426d45b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321907"
---
# <a name="issues-with-links-and-urls"></a>Ζητήματα με συνδέσεις και διευθύνσεις URL

Οι διευθύνσεις URL ανακατεύθυνσης URI/reply (και οι δύο παραστάσεις είναι εναλλάξιμες) είναι οι διευθύνσεις URL που χρησιμοποιούνται από την Πλατφόρμα ταυτοτήτων της Microsoft για την επιστροφή των διακριτικών που ζητήθηκαν από την εφαρμογή. Για πληροφορίες σχετικά με αυτές τις διευθύνσεις URL, ανατρέξτε στα ακόλουθα άρθρα:

- [Ροές ελέγχου ταυτότητας και σενάρια εφαρμογών](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) - Πληροφορίες σχετικά με τις URI ανακατεύθυνσης στη σελίδα **Καταχώρηση εφαρμογής** για κάθε σενάριο.
- [Περιορισμοί και όρια διεύθυνσης URL ανακατεύθυνσης URI/reply](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**Δεν γνωρίζω πώς να καταχωρήσω τη σωστή διεύθυνση URL ανακατεύθυνσης URI/reply για την εφαρμογή μου**

Κατά την είσοδο μέσω της εφαρμογής που αναπτύσσετε, εάν το παράθυρο διαλόγου σύνδεσης εμφανίζει το μήνυμα **AADSTS50011: Η διεύθυνση URL απάντησης που καθορίζεται στο αίτημα δεν συμφωνεί με τις διευθύνσεις URL απαντήσεων που έχουν ρυθμιστεί για την εφαρμογή <your app ID>**, θα πρέπει να προσθέσετε στην εγγραφή της εφαρμογής σας, το URI ανακατεύθυνσης που χρησιμοποίησε ο κώδικάς σας στο αίτημα για διακριτικό στην Πλατφόρμα ταυτοτήτων της Microsoft.

Για να προσθέσετε μια διεύθυνση URL απάντησης, μεταβείτε στην καρτέλα **Έλεγχος ταυτότητας** στη σελίδα **εγγραφής της εφαρμογής** σας στην πύλη Microsoft Azure και προσθέστε μια καταχώρηση στην ενότητα **URI ανακατεύθυνσης**. Η τιμή που πρέπει να εισαγάγετε εξαρτάται από τον τύπο της εφαρμογής που κατασκευάζεται, όπως περιγράφεται παρακάτω:

- Για εφαρμογές μίας σελίδας και για εφαρμογές web, η διεύθυνση URL απάντησης είναι μια διεύθυνση URL στην εφαρμογή σας. Ανατρέξτε στο θέμα [Καταχώρηση εφαρμογής μίας σελίδας](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) ή [Καταχώριση μιας εφαρμογής web χρησιμοποιώντας την πύλη Microsoft Azure](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)
- Για τις εφαρμογές υπολογιστή, η τιμή που πρέπει να επιλέξετε εξαρτάται από τα εξής:
    - την πλατφόρμα (το MacOS είναι διαφορετικό από τα Windows ή το Linux)
    - τον τρόπο με τον οποίο θα αποκτήσετε το διακριτικό (αλληλεπιδραστικά, με ροή κωδικών συσκευής, με Ενσωματωμένο έλεγχο ταυτότητας των Windows [IWA] ή με όνομα χρήστη / κωδικό πρόσβασης).
    Για λεπτομέρειες, ανατρέξτε στο θέμα [Εφαρμογές υπολογιστή - Εγγραφή εφαρμογής - URi ανακατεύθυνσης](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)
- Για τις εφαρμογές για κινητές συσκευές, το URI ανακατεύθυνσης εξαρτάται από:
    - την πλατφόρμα (iOS/Android/UWP)
    - τις πληροφορίες που χρησιμοποιούνται για την κατασκευή της εφαρμογής σας, όπως το αναγνωριστικό πακέτου στο iOS και τον κατακερματισμό πακέτου ονόματος και υπογραφής στο Android. Η εγγραφή στην εφαρμογή της πύλης Microsoft Azure θα σας βοηθήσει. Για λεπτομέρειες, ανατρέξτε στο θέμα [Ρύθμιση παραμέτρων πλατφόρμας και URI ανακατεύθυνσης](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).

**Σημείωση:** Τα API Web και ορισμένοι από τους σιωπηρούς τρόπους απόκτησης διακριτικών (IWA και όνομα χρήστη/κωδικός πρόσβασης) δεν απαιτούν ανακατεύθυνση URI.

**Έχω αναπτύξει την εφαρμογή web μου και όταν δοκιμάζω την ανεπτυγμένη εφαρμογή, εμφανίζεται ένα μήνυμα ασυμφωνίας διεύθυνσης URL απάντησης**

Προσθέστε URI ανακατεύθυνσης για όλες τις θέσεις στις οποίες αναπτύσσετε την εφαρμογή web σας. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Δήλωση μιας εφαρμογής web χρησιμοποιώντας την πύλη Microsoft Azure](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).

**Σημείωση:** Προσθέστε ανακατεύθυνση URI για μια θέση αμέσως μετά την ανάπτυξη της εφαρμογής σε αυτήν τη θέση.

**Δεν μπορώ να καταχωρήσω αρκετές διευθύνσεις URL απάντησης**

Είσαστε ISV και έχετε ένα ή πολλά URI ανακατεύθυνσης για κάθε πελάτη σας. Θέλετε να κάνετε μετεγκατάσταση από το ADAL/Azure AD v1.0 στο MSAL / "την Πλατφόρμα ταυτοτήτων της Microsoft" και πατήσατε τον [μέγιστο αριθμό URI ανακατευθύνσεων](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris). Για να επιλύσετε αυτό το πρόβλημα, [προσθέσετε URI ανακατεύθυνσης σε οντότητες υπηρεσίας](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) που αντιστοιχούν σε κάθε έναν από τους πελάτες σας.
