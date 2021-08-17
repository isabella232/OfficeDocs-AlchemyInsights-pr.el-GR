---
title: Διεκδίκηση SAML (Διακριτικά)
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
ms.openlocfilehash: 9c8ff0d4ff6da98ed6a5c42570d4a5fac80b00e93d1356b298528bd8d2c51a5f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54109240"
---
# <a name="saml-assertions-tokens"></a>Διεκδίκηση SAML (Διακριτικά)

1. Τα διακριτικά γλώσσας σήμανσης διεκδίκων ασφαλείας (SAML) είναι παραστάσεις απαιτήσεων XML. Από προεπιλογή, τα διακριτικά SAML Windows επικοινωνίας (WCF) που χρησιμοποιούνται σε ομόσπονδα σενάρια ασφαλείας εκδίδονται διακριτικά. Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα Διακριτικά SAML και Αξιώσεις.](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims)
2. Η Πλατφόρμα ταυτοτήτων της Microsoft εκπέμπει διάφορους τύπους διακριτικών ασφαλείας κατά την επεξεργασία κάθε ροής ελέγχου ταυτότητας. [Η αναφορά αξιώσεις διακριτικού SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) περιγράφει τη μορφή, τα χαρακτηριστικά ασφαλείας και τα περιεχόμενα των διακριτικών SAML 2.0.
3. Ακολουθήστε τις οδηγίες στο πλαίσιο ["Διάρκεια ζωής διακριτικού](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) με δυνατότητα ρύθμισης παραμέτρων" Πλατφόρμα ταυτοτήτων της Microsoft για να κατανοήσετε πώς μπορείτε να ρυθμίσετε τις παραμέτρους της ζωής διακριτικών.
4. Ακολουθήστε τα βήματα που περιγράφονται σε αυτό [το άρθρο για να](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) κατανοήσετε πώς μπορείτε να ρυθμίσετε τις παραμέτρους κρυπτογράφησης διακριτικού Azure AD SAML.
5. Στο Azure AD, μπορείτε να ρυθμίσετε επιλογές υπογραφής πιστοποιητικού και τον αλγόριθμο υπογραφής πιστοποιητικού. Για περισσότερες πληροφορίες, [ανατρέξτε στο θέμα Επιλογές υπογραφής πιστοποιητικών](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)για προχωρημένους στο διακριτικό SAML για εφαρμογές συλλογής στο Azure Active Directory.
