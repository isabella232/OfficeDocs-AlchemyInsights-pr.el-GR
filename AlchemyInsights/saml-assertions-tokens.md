---
title: Ισχυρισμοί SAML (tokens)
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
- "9004341"
- "7753"
ms.openlocfilehash: 557e23da09df3ab066c2ad7c0352f5fd904b5490
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885214"
---
# <a name="saml-assertions-tokens"></a>Ισχυρισμοί SAML (tokens)

1. Τα κουπόνια ισχυρισμών της γλώσσας σήμανσης ασφαλείας (SAML) είναι παραστάσεις XML για αξιώσεις. Από προεπιλογή, τα διακριτικά SAML που χρησιμοποιούνται για τα Windows Communication Foundation (WCF) στα ομόσπονδα σενάρια ασφαλείας εκδίδονται ως διακριτικά. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [διακριτικά και αξιώσεις του SAML](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).
2. Η πλατφόρμα ταυτοτήτων της Microsoft εκπέμπει διάφορους τύπους διακριτικών ασφαλείας κατά την επεξεργασία κάθε ροής ελέγχου ταυτότητας. [Αναφορά απαιτήσεων διακριτικού SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) περιγράφει τη μορφή, τα χαρακτηριστικά ασφαλείας και τα περιεχόμενα των διακριτικών του SAML 2,0.
3. Ακολουθήστε τις οδηγίες στη [διάρκεια ζωής διακριτικού με δυνατότητα ρύθμισης παραμέτρων στην πλατφόρμα ταυτοτήτων της Microsoft](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) , για να καταλάβετε πώς να ρυθμίσετε τις παραμέτρους των διακριτικών ζωών.
4. Ακολουθήστε τα βήματα που περιγράφονται σε [αυτό το άρθρο](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) για να καταλάβετε πώς να ρυθμίσετε τις παραμέτρους της κρυπτογράφησης του διακριτικού Azure AD SAML.
5. Στο Azure AD, μπορείτε να ρυθμίσετε τις επιλογές υπογραφής πιστοποιητικών και τον αλγόριθμο υπογραφής πιστοποιητικού. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [επιλογές υπογραφής πιστοποιητικών για προχωρημένους στο ΔΙΑΚΡΙΤΙΚΌ SAML για τις εφαρμογές συλλογής στο Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).
