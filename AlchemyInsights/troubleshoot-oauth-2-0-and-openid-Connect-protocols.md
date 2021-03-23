---
title: Αντιμετώπιση προβλημάτων πρωτοκόλλων OAuth 2.0 και OpenID Connect
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9776"
- "9004342"
ms.openlocfilehash: d2f14d4d16bea890b564cdb9bd9ac3875c28d115
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036408"
---
# <a name="troubleshoot-oauth-20-and-openid-connect-protocols"></a>Αντιμετώπιση προβλημάτων πρωτοκόλλων OAuth 2.0 και OpenID Connect

Για να επιλύσετε προβλήματα OAuth 2.0 και OpenID Connect, εκτελέστε τα ακόλουθα προτεινόμενα βήματα:

Ανατρέξτε στα ακόλουθα άρθρα που σχετίζονται με τη ρύθμιση παραμέτρων και την αντιμετώπιση προβλημάτων πρωτοκόλλων OAuth 2.0 και OpenID Connect:

- Πλατφόρμα ταυτότητας της Microsoft και ροή κωδικών εξουσιοδότησης [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) - Αυτό το άρθρο περιγράφει τον τρόπο απευθείας προγραμματισμού με βάση τη ροή εκχώρησης κώδικα **(PKCE)** στην εφαρμογή σας, χρησιμοποιώντας οποιαδήποτε γλώσσα.
- Η πλατφόρμα ταυτότητας της Microsoft και η ροή διαπιστευτηρίων του προγράμματος-πελάτη [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) - Αυτό το άρθρο περιγράφει τον τρόπο με τον οποίο μπορείτε να προγραμματίσετε απευθείας τη ροή των διαπιστευτηρίων του προγράμματος-πελάτη στην εφαρμογή σας. 
- [Microsoft identity platform and OAuth 2.0 Resource Owner Password Credentials](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth-ropc) - This article describes how to program directly against the **ROPC flow** in your application.
    - Η πλατφόρμα ταυτότητας της Microsoft υποστηρίζει μόνο ROPC για μισθωτές Azure AD και όχι για προσωπικούς λογαριασμούς. Αυτό σημαίνει ότι πρέπει να χρησιμοποιήσετε ένα τελικό σημείο συγκεκριμένου μισθωτή **( https://login.microsoftonline.com/{TenantId_or_Name})** ή **το τελικό σημείο των** οργανισμών.
    - Οι προσωπικοί λογαριασμοί που έχουν προσκληθεί σε ένα μισθωτή Azure AD δεν μπορούν να χρησιμοποιήσουν ropc.
    - Οι λογαριασμοί που δεν έχουν κωδικούς πρόσβασης δεν μπορούν να πραγματοποιήσουν είσοδο μέσω ROPC. Για αυτό το σενάριο, συνιστάται να χρησιμοποιήσετε μια διαφορετική ροή για την εφαρμογή σας.
    - Εάν οι χρήστες πρέπει να χρησιμοποιήσουν έλεγχο ταυτότητας πολλών παραγόντων [(MFA)](https://docs.microsoft.com/azure/active-directory/authentication/concept-mfa-howitworks) για να συνδεθούν στην εφαρμογή, θα αποκλείονται.
    - Η ropc δεν υποστηρίζεται σε [σενάρια ομοσπονδίας υβριδικής](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-fed) ταυτότητας (για παράδειγμα, το Azure AD και το ADFS που χρησιμοποιούνται για τον έλεγχο ταυτότητας λογαριασμών εσωτερικής εγκατάστασης). Εάν οι χρήστες ανακατευθυνθούν σε πλήρη σελίδα σε μια υπηρεσία παροχής ταυτότητας εσωτερικής εγκατάστασης, το Azure AD δεν μπορεί να δοκιμάσει το όνομα χρήστη και τον κωδικό πρόσβασης σε αυτήν την υπηρεσία παροχής ταυτότητας. [Ωστόσο, ο έλεγχος ταυτότητας](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-pta) μέσω πρόσβασης υποστηρίζεται με ropc.
    - Μια εξαίρεση σε ένα σενάριο ομοσπονδίας υβριδικής ταυτότητας θα ήταν το εξής: Η πολιτική εντοπισμού τομέα οικίας με το **AllowCloudPasswordValidation** να έχει οριστεί σε **TRUE** θα επιτρέψει τη λειτουργία της ροής ROPC για ομόσπονδους χρήστες όταν ο κωδικός πρόσβασης εσωτερικής εγκατάστασης συγχρονίζεται στο cloud. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Ενεργοποίηση άμεσου ελέγχου ταυτότητας ROPC ομόσπονδων χρηστών για εφαρμογές παλαιού τύπου](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#enable-direct-ropc-authentication-of-federated-users-for-legacy-applications) 
- [Πλατφόρμα ταυτότητας της Microsoft και ροή OAuth 2.0 On-Behalf-Of](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow) - Αυτό το άρθρο περιγράφει τον τρόπο με τον οποίο μπορείτε να προγραμματίσετε απευθείας σε σχέση με τη ροή εκ μέρους **του (OBO)** στην εφαρμογή σας.
- [Πλατφόρμα ταυτότητας της Microsoft](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) και πρωτόκολλο OpenID Connect - Αυτό το άρθρο δείχνει πώς μπορείτε να υλοποιήσετε το πρωτόκολλο OpenID Connect ανεξάρτητα από τη γλώσσα και περιγράφει πώς μπορείτε να στέλνετε και να λαμβάνετε μηνύματα HTTP χωρίς να χρησιμοποιείτε βιβλιοθήκες ανοιχτού κώδικα της Microsoft.

**Διακριτικά της Access**

[Διακριτικά πρόσβασης πλατφόρμας ταυτότητας της Microsoft](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) - Μάθετε πώς το API σας μπορεί να επικυρώσει και να χρησιμοποιήσει τις αξιώσεις μέσα σε ένα διακριτικό πρόσβασης. Όλη η τεκμηρίωση σε αυτό το άρθρο, εκτός εάν αναφέρεται, ισχύει μόνο για τα διακριτικά που έχουν εκδοθεί για API που έχετε καταχωρηθεί. Δεν ισχύει για τα διακριτικά που εκδίδονται για API που ανήκουν στη Microsoft, ούτε μπορούν αυτά τα διακριτικά να χρησιμοποιηθούν για την επικύρωση του πώς η πλατφόρμα ταυτότητας της Microsoft θα εκδίδει διακριτικά για ένα API που δημιουργείτε.

**Ρύθμιση παραμέτρων εφαρμογής**

[Περιορισμοί και περιορισμοί ανακατεύθυνσης URI (διεύθυνση URL απάντησης)](https://docs.microsoft.com/azure/active-directory/develop/reply-url) - Μάθετε πώς μπορείτε να ρυθμίσετε τις παραμέτρους του URI ανακατεύθυνσης (διεύθυνση URL απάντησης). Ένα URI ανακατεύθυνσης ή μια διεύθυνση URL απάντησης είναι η θέση όπου ο διακομιστής εξουσιοδότησης στέλνει το χρήστη μετά την επιτυχή εξουσιοδότηση της εφαρμογής και της έχει παραχωρηθεί κωδικός εξουσιοδότησης ή διακριτικό πρόσβασης. Ο διακομιστής εξουσιοδότησης στέλνει τον κωδικό ή το διακριτικό στο URI ανακατεύθυνσης. επομένως, είναι σημαντικό να καταχωρήσετε τη σωστή θέση ως μέρος της διαδικασίας εγγραφής της εφαρμογής.

**Προμήθεια εφαρμογών**

[Πρόγραμμα εκμάθησης:](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) Ανάπτυξη και σχεδιασμός παροχής για ένα τελικό σημείο SCIM - Αυτό το άρθρο περιγράφει πώς μπορείτε να δημιουργήσετε ένα τελικό σημείο SCIM και να ενοποιηθείτε με την υπηρεσία παροχής AAD.


