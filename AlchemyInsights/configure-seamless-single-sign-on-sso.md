---
title: Ρύθμιση παραμέτρων απρόσκοπτη ενιαία σύνδεση (SSO)
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004344"
- "9004357"
- "9384"
- "9863"
ms.openlocfilehash: bd3873c2db1b8d548f81d531a8bf5747130fe761
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402267"
---
# <a name="configure-seamless-single-sign-on-sso"></a>Ρύθμιση παραμέτρων απρόσκοπτη ενιαία σύνδεση (SSO)

**Ρύθμιση παραμέτρων εφαρμογών**

1. Θα πρέπει να λάβετε τις τιμές από τον προμηθευτή της εφαρμογής. Μπορείτε να εισαγάγετε τις τιμές με μη αυτόματο τρόπο ή να αποστείλετε ένα αρχείο μετα-δεδομένων για να εξαγάγετε την τιμή των πεδίων.
2. Πολλές εφαρμογές έχουν ήδη ρυθμιστεί εκ των προ-παραμέτρων για να λειτουργούν με το Azure AD. Αυτές οι εφαρμογές παρατίθενται στη συλλογή των εφαρμογών που μπορείτε να αναζητήσετε όταν προσθέτετε μια εφαρμογή στο μισθωτή Azure AD. Η [σειρά γρήγορης εκκίνησης σας](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) παρέχει τη διαδικασία.
3. Για να δημιουργήσετε μια εφαρμογή που δεν είναι συλλογή, μπορείτε να κάνετε κλικ στο + Δημιουργία του κουμπιού **"Εφαρμογή"** και να δώσετε ένα όνομα στην εφαρμογή σας.
    - Από προεπιλογή, θα επιλέξει **"Ενοποίηση"** κάθε άλλης εφαρμογής που δεν βρίσκετε στη συλλογή, η οποία είναι η σωστή επιλογή για τις εφαρμογές που δεν είναι συλλογή.
    - Αφού κατόπιν **κατόπιν** την επιλογή "Δημιουργία" μετά την τοποθέτηση του ονόματος για την εφαρμογή, θα δημιουργηθεί μια νέα εταιρική εφαρμογή που δεν είναι συλλογή.
    - Στη συνέχεια, μπορείτε  να μεταβείτε  στην επιλογή "Ενιαία σύνδεση" στην περιοχή "Διαχείριση αυτής της εφαρμογής" και θα μπορείτε να δείτε διαφορετικές τεχνικές για την εφαρμογή της στο περιβάλλον σας.

**Ρύθμιση παραμέτρων απρόσκοπτη SSO για μια συγκεκριμένη εφαρμογή**

Για τις εφαρμογές στη συλλογή θα βρείτε λεπτομερείς οδηγίες, βήμα προς βήμα. Για να αποκτήσετε πρόσβαση στα βήματα, μπορείτε να περιηγηθείτε σε μια λίστα με όλα τα προγράμματα εκμάθησης ρύθμισης παραμέτρων εφαρμογών στα προγράμματα εκμάθησης ρύθμισης παραμέτρων [της εφαρμογής SaaS.](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list)

**Ρύθμιση παραμέτρων SSO που βασίζεται σε SAML**

1. Γρήγορη εκκίνηση: Ρυθμίστε την ενιαία σύνδεση [(SSO) που](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso)βασίζεται σε SAML για μια εφαρμογή στο μισθωτή Azure Active Directory (Azure AD).
2. Για να μάθετε περισσότερα σχετικά με την επιλογή που βασίζεται σε SAML για μία σύνδεση, ανατρέξτε στο θέμα Κατανόηση της μεμονωμένης sign-on που βασίζεται [σε SAML.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on)
3. Για να μάθετε περισσότερα σχετικά με τις αιτήσεις ελέγχου ταυτότητας SAML 2.0 και τις αποκρίσεις που υποστηρίζει το Azure Active Directory (Azure AD) για το Single Sign-On (SSO), ανατρέξτε στο [Sign-On πρωτόκολλο SAML.](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
4. Για να μάθετε πώς μπορείτε να δημιουργήσετε και να ρυθμίσετε τις παραμέτρους μιας μεμονωμένης σύνδεσης (SSO) που βασίζεται σε SAML για την εφαρμογή σας στο Azure Active Directory (Azure AD) χρησιμοποιώντας το API του Microsoft Graph, ανατρέξτε στο θέμα Ρύθμιση παραμέτρων μίας σύνδεσης που βασίζεται σε SAML για την εφαρμογή σας χρησιμοποιώντας το [API του Microsoft Graph.](https://docs.microsoft.com/graph/application-saml-sso-configure-api)
5. Για να μάθετε πώς το Azure AD χρησιμοποιεί το πρωτόκολλο SAML, ανατρέξτε στο θέμα [Πώς η πλατφόρμα ταυτότητας της Microsoft χρησιμοποιεί το πρωτόκολλο SAML.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference)

**Ρύθμιση παραμέτρων διακριτικών και αξιώσεις**

1. [Τρόπος: προσαρμογή αξιώ σεων που εκδίδονται στο διακριτικό SAML για εταιρικές εφαρμογές.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)
2. Για να μάθετε πώς μπορείτε να ρυθμίσετε τις παραμέτρους αξιώσεών σας χρησιμοποιώντας το PowerShell, ανατρέξτε στο θέμα Τρόπος: Προσαρμογή αξιώσεών που εκπεμπόμενων σε διακριτικά για μια συγκεκριμένη εφαρμογή σε [ένα μισθωτή (Προεπισκόπηση).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)
3. Για να μάθετε πώς μπορείτε να ρυθμίσετε τις παραμέτρους προαιρετικών αξιώσεις, ανατρέξτε στο θέμα [Πώς να: Παρέχετε προαιρετικές αξιώσεις στην εφαρμογή σας.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)
4. Για να μάθετε πώς μπορείτε να χρησιμοποιήσετε τα χαρακτηριστικά επέκτασης σχήματος καταλόγου για την αποστολή δεδομένων χρήστη σε εφαρμογές σε αξιώσεις διακριτικού, ανατρέξτε στο θέμα Χρήση χαρακτηριστικών επέκτασης [σχήματος καταλόγου σε αξιώσεις.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions)
5. Για να μάθετε πώς μπορείτε να ρυθμίσετε τις παραμέτρους της ζωής διακριτικού, ανατρέξτε στο θέμα "Διάρκεια ζωής διακριτικού με δυνατότητα ρύθμισης παραμέτρων" στην [πλατφόρμα ταυτότητας της Microsoft (προεπισκόπηση).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)
6. [Ρύθμιση παραμέτρων πολιτικών διάρκειας ζωής διακριτικού (προεπισκόπηση)](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) - Σε αυτό το άρθρο, θα σας βοηθήσουμε να επιβάλετε νέους κανόνες για τη διάρκεια ζωής του διακριτικού. Στο παράδειγμα, θα μάθετε πώς μπορείτε να δημιουργήσετε μια πολιτική που απαιτεί από τους χρήστες να ελέγχουν τον έλεγχο ταυτότητας πιο συχνά στην εφαρμογή web.

**Αντιμετώπιση προβλημάτων ρύθμισης παραμέτρων SSO**

- Για συνήθεις ερωτήσεις σχετικά με το Azure Active Directory Seamless Single Sign-On (Απρόσκοπτη SSO), ανατρέξτε στο θέμα "Απρόσκοπτη ενιαία σύνδεση" της υπηρεσίας καταλόγου [Azure Active Directory: Συνήθεις ερωτήσεις.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq)
- Για πληροφορίες αντιμετώπισης προβλημάτων σχετικά με συνήθη προβλήματα σχετικά με το Azure Active Directory (Azure AD) Απρόσκοπτη ενιαία Sign-On (Απρόσκοπτη SSO), ανατρέξτε στο θέμα Αντιμετώπιση προβλημάτων απρόσκοπτης μεμονωμένης σύνδεσης του [Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso)
