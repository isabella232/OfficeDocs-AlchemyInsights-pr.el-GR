---
title: Προβλήματα με τα κουπόνια
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
- "7774"
- "9004351"
ms.openlocfilehash: 14a9681c08920094813497e7a75eb87bb0733cbc
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/20/2021
ms.locfileid: "49916843"
---
# <a name="issues-with-tokens"></a>Προβλήματα με τα κουπόνια

Για να διαχειριστείτε θέματα που σχετίζονται με τα token, μπορείτε να ακολουθήσετε τα παρακάτω βήματα:

1. Μπορείτε να καθορίσετε τη διάρκεια ζωής ενός διακριτικού Access, ID ή SAML που έχει εκδοθεί από την πλατφόρμα ταυτοτήτων της Microsoft. Μπορείτε να καθορίσετε τη διάρκεια ζωής διακριτικού για όλες τις εφαρμογές στον οργανισμό σας, για μια εφαρμογή πολλαπλών μισθωτών (πολλών οργανισμών) ή για μια συγκεκριμένη κύρια υπηρεσία στην εταιρεία σας. Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα διάρκεια ζωής διακριτικού με δυνατότητα ρύθμισης παραμέτρων στην πλατφόρμα ταυτοτήτων της Microsoft (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
2. Οι κωδικοί πρόσβασης επιτρέπουν στους υπολογιστές-πελάτες να καλέσουν με ασφάλεια τα προστατευμένα API Web και χρησιμοποιούνται από τα API Web για την εκτέλεση ελέγχου ταυτότητας και εξουσιοδότησης. Σύμφωνα με την προδιαγραφή OAuth, οι κωδικοί πρόσβασης είναι αδιαφανείς συμβολοσειρές χωρίς μορφή συνόλου-ορισμένες υπηρεσίες παροχής ταυτότητας (εκτοπισμένοι) χρησιμοποιούν GUID, ενώ άλλα χρησιμοποιούν κρυπτογραφημένες σταγόνες. Η πλατφόρμα ταυτοτήτων της Microsoft χρησιμοποιεί μια ποικιλία μορφών διακριτικού πρόσβασης, ανάλογα με τη ρύθμιση παραμέτρων του API που αποδέχεται το διακριτικό. Για να μάθετε πώς το API σας μπορεί να επικυρώσει και να χρησιμοποιήσει τις αξιώσεις μέσα σε ένα διακριτικό πρόσβασης, ανατρέξτε στο θέμα [διακριτικά πρόσβασης στην πλατφόρμα ταυτοτήτων της Microsoft](https://docs.microsoft.com/azure/active-directory/develop/userinfo#calling-the-userinfo-endpoint).
3. Η βιβλιοθήκη ελέγχου ταυτότητας της Microsoft (MSAL) υποστηρίζει διάφορες ροές ελέγχου ταυτότητας για χρήση σε διαφορετικά σενάρια εφαρμογής. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [ροές ελέγχου ταυτότητας](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows#how-each-flow-emits-tokens-and-codes).
4. Η επιχορήγηση του κωδικού εξουσιοδότησης OAuth 2,0 μπορεί να χρησιμοποιηθεί σε εφαρμογές που είναι εγκατεστημένες σε μια συσκευή για να αποκτήσουν πρόσβαση σε προστατευμένους πόρους, όπως τα API Web. Χρησιμοποιώντας την εφαρμογή πλατφόρμας ταυτοτήτων της Microsoft του OAuth 2,0, μπορείτε να προσθέσετε πρόσβαση εισόδου και API σε κινητές συσκευές και εφαρμογές υπολογιστή. Ανατρέξτε στο θέμα [ροή κωδικού εξουσιοδότησης για την πλατφόρμα Microsoft Identity και OAuth 2,0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow#refresh-the-access-token) για τον τρόπο με τον οποίο μπορείτε να προγραμματίσετε απευθείας το πρωτόκολλο στην εφαρμογή σας, χρησιμοποιώντας οποιαδήποτε γλώσσα.
5. Το OpenID Connect (OIDC) είναι ένα πρωτόκολλο ελέγχου ταυτότητας που είναι ενσωματωμένο στο OAuth 2,0, το οποίο μπορείτε να χρησιμοποιήσετε για να συνδεθείτε με ασφάλεια σε ένα χρήστη σε μια εφαρμογή. Όταν χρησιμοποιείτε την εφαρμογή απόληξης πλατφόρμας Microsoft Identity της OpenID Connect, μπορείτε να προσθέσετε πρόσβαση εισόδου και API στις εφαρμογές σας. Το [Πρωτόκολλο Microsoft Identity Platform και OpenID Connect](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc#send-the-sign-in-request) δείχνει πώς μπορείτε να το κάνετε αυτό ανεξάρτητα από τη γλώσσα και περιγράφει τον τρόπο με τον οποίο μπορείτε να στέλνετε και να ΛΑΜΒΆΝΕΤΕ μηνύματα HTTP χωρίς να χρησιμοποιείτε βιβλιοθήκες ανοιχτού κώδικα της Microsoft.
    - Το τελικό σημείο UserInfo αποτελεί μέρος του προτύπου OIDC, το οποίο έχει σχεδιαστεί για να επιστρέφει αξιώσεις σχετικά με το χρήστη με τον οποίο έγινε έλεγχος ταυτότητας. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [απόληξη του Microsoft Identity Platform UserInfo](https://docs.microsoft.com/azure/active-directory/develop/userinfo#consider-use-an-id-token-instead).
    - Η [κλήση ΕΝΌς API Web σε μια εφαρμογή Web με τη χρήση του δείγματος Azure AD και OpenID Connect](https://docs.microsoft.com/samples/azure-samples/active-directory-dotnet-webapp-webapi-openidconnect/active-directory-dotnet-webapp-webapi-openidconnect/) δείχνει πώς μπορείτε να δημιουργήσετε μια εφαρμογή Web MVC που χρησιμοποιεί το Azure AD για είσοδο χρησιμοποιώντας το πρωτόκολλο σύνδεσης του OpenID και, στη συνέχεια, να ΚΑΛΈΣΕΤΕ ένα API Web κάτω από την ταυτότητα του χρήστη που έχει συνδεθεί με τη χρήση διακριτικών που έχουν ληφθεί μέσω του OAuth 2,0. Αυτό το δείγμα χρησιμοποιεί το OpenID Connect ASP .NET OWIN ενδιάμεσα και ADAL .NET.
6. [Ρύθμιση παραμέτρων μιας εφαρμογής για να εκθέσετε ένα API Web](https://docs.microsoft.com/azure/active-directory/develop/quickstart-configure-app-expose-web-apis) -σε αυτήν την γρήγορη εκκίνηση, καταχωρείτε ένα API Web με την πλατφόρμα ταυτοτήτων της Microsoft και το εκθέτετε σε εφαρμογές υπολογιστή-πελάτη, προσθέτοντας ένα παράδειγμα εμβέλειας. Με την καταχώρηση του API Web και την έκθεσή του μέσω εύρους, μπορείτε να παρέχετε πρόσβαση με βάση τα δικαιώματα στους πόρους της σε εξουσιοδοτημένους χρήστες και εφαρμογές υπολογιστή-πελάτη που έχουν πρόσβαση στο API σας.
7. Στο Azure Active Directory B2C (Azure AD B2C), η ροή διαπιστευτηρίων κωδικού πρόσβασης κατόχου πόρου (ROPC) είναι μια τυπική ροή ελέγχου ταυτότητας OAuth. Σε αυτήν τη ροή, μια εφαρμογή, γνωστή και ως ομάδα επικαλούμενη, ανταλλάσσει έγκυρα διαπιστευτήρια για τα token. Τα διαπιστευτήρια περιλαμβάνουν ένα αναγνωριστικό χρήστη και έναν κωδικό πρόσβασης. Τα διακριτικά που επιστρέφονται είναι ένα διακριτικό ΑΝΑΓΝΩΡΙΣΤΙΚού, ένα διακριτικό πρόσβασης και ένα διακριτικό ανανέωσης. Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα Ρύθμιση διαπιστευτηρίων κωδικού πρόσβασης κατόχου πόρου στο πρόγραμμα Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/add-ropc-policy?tabs=app-reg-ga&pivots=b2c-user-flow). 
