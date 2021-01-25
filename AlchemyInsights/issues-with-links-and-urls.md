---
title: Προβλήματα με συνδέσεις και διευθύνσεις URL
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: 24885d873d6471a72ae66581ad1ceb0a19b664f7
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974463"
---
# <a name="issues-with-links-and-urls"></a>Προβλήματα με συνδέσεις και διευθύνσεις URL

Ανακατεύθυνση διευθύνσεων URL URI/απαντήσεων (και οι δύο παραστάσεις είναι εναλλάξιμες) είναι οι διευθύνσεις URL που χρησιμοποιούνται από την πλατφόρμα ταυτοτήτων της Microsoft για την επιστροφή διακριτικών που ζητήθηκαν από την εφαρμογή. Για πληροφορίες σχετικά με αυτές τις διευθύνσεις URL, ανατρέξτε στα ακόλουθα άρθρα:

- [Ροές ελέγχου ταυτότητας και σενάρια εφαρμογών](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) -πληροφορίες σχετικά με τα URI ανακατεύθυνσης στη σελίδα **καταχώρησης εφαρμογών** για κάθε σενάριο.
- [Ανακατεύθυνση URI/απαντήσεων διευθύνσεων URL και περιορισμών](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**Δεν γνωρίζω πώς να καταχωρήσω τη σωστή ανακατεύθυνση της διεύθυνσης URL URI/απάντησης για την εφαρμογή μου**

Όταν πραγματοποιείτε είσοδο με την εφαρμογή που αναπτύσσετε, εάν το παράθυρο διαλόγου εισόδου εμφανίζει το **AADSTS50011: η διεύθυνση URL απάντησης που καθορίζεται στην αίτηση δεν συμφωνεί με τις ρυθμίσεις URL απαντήσεων που έχουν <your app ID> ρυθμιστεί για την εφαρμογή**, θα πρέπει να προσθέσετε στην καταχώρηση της εφαρμογής σας, το URI ανακατεύθυνσης που χρησιμοποιεί ο κώδικάς σας στην αίτηση διακριτικού στην πλατφόρμα ταυτοτήτων της Microsoft.

Για να προσθέσετε μια διεύθυνση URL απάντησης, μεταβείτε στην καρτέλα **Έλεγχος ταυτότητας** στη σελίδα **δήλωσης της εφαρμογής** σας στην πύλη Azure και προσθέστε μια καταχώρηση στην ενότητα **ανακατεύθυνση URI** . Τα URI ανακατεύθυνσης πληκτρολογούνται (Web ή Mobile/Desktop). Η τιμή που θέλετε να εισαγάγετε εξαρτάται από τον τύπο της εφαρμογής που δημιουργείτε, όπως περιγράφεται παρακάτω:

- Για εφαρμογές μίας σελίδας και εφαρμογές Web, η διεύθυνση URL απάντησης είναι μια διεύθυνση URL στην εφαρμογή σας. Ανατρέξτε στο θέμα [καταχώρηση εφαρμογής μίας σελίδας](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) ή [καταχώρηση μιας εφαρμογής Web App με χρήση της πύλης Azure](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)
- Για εφαρμογές υπολογιστή, η τιμή που πρέπει να επιλέξετε εξαρτάται από:
    - η πλατφόρμα (το MacOS είναι διαφορετικό από τα Windows ή το Linux)
    - ο τρόπος με τον οποίο αποκτάτε το διακριτικό (αλληλεπιδραστικά, με τη ροή κώδικα συσκευής, με ενσωματωμένο έλεγχο ταυτότητας των Windows [IWA] ή με όνομα χρήστη/κωδικό πρόσβασης).
    Για λεπτομέρειες, ανατρέξτε [στο θέμα εφαρμογές υπολογιστή-καταχώρηση εφαρμογής-URi ανακατεύθυνσης](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)
- Για εφαρμογές για κινητές συσκευές, το URI ανακατεύθυνσης εξαρτάται από:
    - η πλατφόρμα (iOS/Android/UWP)
    - Οι πληροφορίες που χρησιμοποιούνται για τη δόμηση της εφαρμογής σας, όπως το αναγνωριστικό δέσμης στο iOS, καθώς και το όνομα του πακέτου και το hash υπογραφής στο Android η καταχώρηση της εφαρμογής Azure Portal θα σας βοηθήσουν. Για λεπτομέρειες, ανατρέξτε στο θέμα [Ρύθμιση παραμέτρων πλατφόρμας και ανακατεύθυνση URI](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).

> [!NOTE]
> Τα API Web και ορισμένοι από τους σιωπηλούς τρόπους απόκτησης διακριτικών (IWA και username/password) δεν απαιτούν URI ανακατεύθυνσης.

**Έχω αναπτύξει την εφαρμογή Web μου και όταν δοκιμάζω την εφαρμογή ανάπτυξης, παίρνω ένα μήνυμα ασυμφωνίας διεύθυνσης URL απάντησης**

Προσθέστε URI ανακατεύθυνσης για όλες τις θέσεις στις οποίες αναπτύσσετε την εφαρμογή Web. Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα καταχώρηση εφαρμογής Web App με χρήση της πύλης Azure](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).

> [!NOTE]
> Προσθήκη URI ανακατεύθυνσης για μια θέση αμέσως μετά την ανάπτυξη της εφαρμογής σε αυτήν τη θέση.

**Δεν μπορώ να καταχωρήσω αρκετές διευθύνσεις URL απαντήσεων**

Είστε ένας ISV και έχετε ένα ή περισσότερα URI ανακατεύθυνσης για κάθε πελάτη σας. Θέλετε να κάνετε μετεγκατάσταση από το ADAL/Azure AD v 1.0 σε MSAL/την πλατφόρμα ταυτοτήτων της Microsoft και να πατήσετε τον [μέγιστο αριθμό των URI ανακατεύθυνσης](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris). Για να επιλύσετε αυτό το συγκεκριμένο, [Προσθέστε URI ανακατεύθυνσης σε αρχές υπηρεσίας](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) που αντιστοιχούν σε κάθε έναν από τους πελάτες σας.
