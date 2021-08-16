---
title: Προβλήματα με αξιώσεις διακριτικού και χαρακτηριστικά
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
ms.openlocfilehash: 0c9827ee312d6b236c86f5a2973fa61fdc78c49b8565dd4ceb41f9a3a48140bc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54012884"
---
# <a name="issues-with-token-claims-and-attributes"></a>Προβλήματα με αξιώσεις διακριτικού και χαρακτηριστικά

**Ενημέρωση, ρύθμιση παραμέτρων ή κατάργηση αξιώ σεων διακριτικού**

1. Χρησιμοποιώντας το Azure Active Directory (Azure AD), [](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) μπορείτε να προσαρμόσετε τον τύπο αξίωσης για την αξίωση ρόλου στο διακριτικό απάντησης που λαμβάνετε μετά την εξουσιοδότηση μιας εφαρμογής.
2. Οι προγραμματιστές εφαρμογών μπορούν να χρησιμοποιήσουν προαιρετικές αξιώσεις στις εφαρμογές Azure AD για να καθορίσουν ποιες αξιώσεις θέλουν σε διακριτικά που αποστέλλονται στην εφαρμογή τους. Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα Παροχή προαιρετικών αξιώσεις στην εφαρμογή σας.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)
3. [Ρυθμίστε τις παραμέτρους αξιώσεις ομάδας για εφαρμογές με Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims)
4. Εάν χρησιμοποιείτε απρόσκοπτη ενιαία σύνδεση στην εφαρμογή σας, ανατρέξτε στο θέμα προσαρμογή αξιώ σεων που εκδίδονται στο [διακριτικό SAML για εταιρικές εφαρμογές.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)

**Αντιστοίχιση χαρακτηριστικού αξιώσεις**

1. Για να ρυθμίσετε τις παραμέτρους της πολιτικής αντιστοίχισης αξιωμάτων χρησιμοποιώντας το PowerShell, ανατρέξτε στο θέμα Προσαρμογή αξιώσεών που εκπεμπόμενων σε διακριτικά για μια συγκεκριμένη [εφαρμογή σε ένα μισθωτή (Προεπισκόπηση).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)
2. Τα χαρακτηριστικά επέκτασης σχήματος καταλόγου παρέχουν έναν τρόπο για την αποθήκευση πρόσθετων δεδομένων Azure Active Directory σε αντικείμενα χρήστη και άλλα αντικείμενα καταλόγου, όπως ομάδες, λεπτομέρειες μισθωτή, αρχές υπηρεσίας. Μόνο τα χαρακτηριστικά επέκτασης σε αντικείμενα χρηστών μπορούν να χρησιμοποιηθούν για την εκπομπή αξιώ σεων σε εφαρμογές. [Η χρήση χαρακτηριστικών επέκτασης σχήματος καταλόγου σε αξιώσεις](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) περιγράφει πώς μπορείτε να χρησιμοποιήσετε χαρακτηριστικά επέκτασης σχήματος καταλόγου για την αποστολή δεδομένων χρήστη σε εφαρμογές με αξιώσεις διακριτικού.

Για περισσότερες πληροφορίες σχετικά με τις αξιώσεις διακριτικού, ανατρέξτε στο θέμα:

- [Αξιώσεις σε διακριτικά πρόσβασης](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [Αξιώσεις σε id_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [Αξιώσεις](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) που μπορείτε να αναμένετε σε διακριτικά αναγνωριστικών και διακριτικά πρόσβασης που εκδίδονται από το Azure AD B2C
- [Αναφορά αξιώ σεων διακριτικού SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
