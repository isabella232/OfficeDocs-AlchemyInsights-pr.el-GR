---
title: Προβλήματα με τις αξιώσεις και τα χαρακτηριστικά διακριτικού
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
- "9004347"
- "7761"
ms.openlocfilehash: 4c12f768ab4bf4547f48abc19736743fa555c477
ms.sourcegitcommit: c1c6047ec467853dc823a17b02c461a6a476406d
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50035891"
---
# <a name="issues-with-token-claims-and-attributes"></a>Προβλήματα με τις αξιώσεις και τα χαρακτηριστικά διακριτικού

**Ενημέρωση, ρύθμιση παραμέτρων ή κατάργηση αξιώσεις διακριτικού**

1. Χρησιμοποιώντας το Azure Active Directory (Azure AD), μπορείτε να προσαρμόσετε τον τύπο αξίωσης για την αξίωση ρόλου στο διακριτικό απάντησης που λαμβάνετε μετά την εξουσιοδότηση μιας εφαρμογής. [](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management)
2. Οι προγραμματιστές εφαρμογών μπορούν να χρησιμοποιήσουν προαιρετικές αξιώσεις στις εφαρμογές του Azure AD για να καθορίσουν ποιες αξιώσεις θέλουν στα διακριτικά που αποστέλλονται στην εφαρμογή τους. Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα "Παροχή προαιρετικών αξιώ σεων στην εφαρμογή σας".](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)
3. [Ρυθμίστε τις παραμέτρους αξιώσεις ομάδας για εφαρμογές με το Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims)
4. Εάν χρησιμοποιείτε απρόσκοπτη σύνδεση μονής πρόσβασης στην εφαρμογή σας, ανατρέξτε στις αιτήσεις προσαρμογής που εκδίδονται στο [διακριτικό SAML για τις εφαρμογές για μεγάλες επιχειρήσεις.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)

**Αντιστοίχιση χαρακτηριστικών διεκδίκησης**

1. Για να ρυθμίσετε τις παραμέτρους πολιτικής αντιστοίχισης αξιώσεις χρησιμοποιώντας το PowerShell, ανατρέξτε στο θέμα "Προσαρμογή αξιώσεων που μεταδίδονται σε διακριτικά για μια συγκεκριμένη εφαρμογή [σε ένα μισθωτή (Προεπισκόπηση)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).
2. Τα χαρακτηριστικά επέκτασης σχήματος καταλόγου παρέχουν έναν τρόπο για την αποθήκευση πρόσθετων δεδομένων στο Azure Active Directory σε αντικείμενα χρηστών και άλλα αντικείμενα καταλόγου, όπως ομάδες, λεπτομέρειες μισθωτή, αρχές υπηρεσίας. Μόνο τα χαρακτηριστικά επέκτασης στα αντικείμενα χρήστη μπορούν να χρησιμοποιηθούν για την εμφάνιση αξιώ σε εφαρμογές. [Η χρήση χαρακτηριστικών επέκτασης σχήματος καταλόγου σε αξιώσεις](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) περιγράφει πώς μπορείτε να χρησιμοποιήσετε χαρακτηριστικά επέκτασης σχήματος καταλόγου για την αποστολή δεδομένων χρήστη σε εφαρμογές σε αξιώσεις διακριτικού.

Για περισσότερες πληροφορίες σχετικά με τις αξιώσεις διακριτικού, ανατρέξτε στα εξής:

- [Αξιώσεις σε διακριτικά πρόσβασης](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [Αξιώσεις σε id_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [Αξιώσεις](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) που μπορείτε να αναμένετε από τα διακριτικά αναγνωριστικού και τα διακριτικά πρόσβασης που εκδίδονται από το Azure AD B2C
- [Αναφορά αξιώ σεων διακριτικού SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
