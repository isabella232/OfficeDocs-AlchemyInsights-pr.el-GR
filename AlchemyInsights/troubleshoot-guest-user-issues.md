---
title: Αντιμετώπιση προβλημάτων χρήστη επισκέπτη
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004358"
- "7822"
ms.openlocfilehash: 9e6030919721b4c0805a26ca45d365f31d88894e86ea08225f47576e7d152047
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939379"
---
# <a name="troubleshoot-guest-user-issues"></a>Αντιμετώπιση προβλημάτων χρήστη επισκέπτη

1. Για οδηγίες σχετικά με τη διαχείριση της πρόσβασης επισκέπτη σε εφαρμογές, ανατρέξτε στο θέμα Διαχείριση πρόσβασης [επισκέπτη με κριτικές πρόσβασης στο Azure AD.](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews)
1. [Προσθέστε χρήστες-επισκέπτες](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal)στον κατάλογο στην πύλη Azure: Σε αυτή τη γρήγορη εκκίνηση, θα προσθέσετε έναν νέο χρήστη-επισκέπτη στον κατάλογο Azure AD μέσω της πύλης Azure, θα στείλετε μια πρόσκληση και θα δείτε πώς μοιάζει η διαδικασία εξαργύρωσης πρόσκλησης του χρήστη-επισκέπτη.
1. [Προσθέστε έναν χρήστη-επισκέπτη](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell)με το PowerShell: Σε αυτή τη γρήγορη εκκίνηση, θα χρησιμοποιήσετε την εντολή New-AzureADMSInvitation για να προσθέσετε έναν χρήστη-επισκέπτη στο μισθωτή Azure.
1. Για να μάθετε πώς μπορείτε να αντιστοιχίσετε χρήστες και ομάδες σε εταιρικές εφαρμογές στο Azure Active Directory (Azure AD), είτε μέσα από την πύλη Azure είτε χρησιμοποιώντας το PowerShell, ανατρέξτε στο θέμα Διαχείριση ανάθεσης χρηστών για μια εφαρμογή [στο Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal) 
1. Azure Active Directory συνεργασίας (Azure AD) B2B λειτουργεί με τις περισσότερες εφαρμογές που ενοποιούνται με το Azure AD. Σε αυτό [το άρθρο,](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)θα σας χρησιμοποιήσουμε οδηγίες για τη ρύθμιση ορισμένων δημοφιλών εφαρμογών SaaS για χρήση με το Azure AD B2B.
1. Ως οργανισμός που χρησιμοποιεί δυνατότητες συνεργασίας Azure Active Directory (Azure AD) B2B για να προσκαλέσει χρήστες-επισκέπτες από οργανισμούς-συνεργάτες στο Azure AD, μπορείτε πλέον να παρέχετε σε αυτούς τους χρήστες B2B πρόσβαση σε εφαρμογές εσωτερικής εγκατάστασης. Αυτές οι εφαρμογές εσωτερικής εγκατάστασης μπορούν να χρησιμοποιούν έλεγχο ταυτότητας που βασίζεται σε SAML ή ενσωματωμένο έλεγχο ταυτότητας Windows (IWA) με περιορισμένη ανάθεση Kerberos (KCD). Για περισσότερες πληροφορίες, [ανατρέξτε στο θέμα Εκχώρηση χρηστών B2B στο Azure AD στις εφαρμογές εσωτερικής εγκατάστασης.](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises)
1. Μάθετε πώς μπορείτε να [εκχωρήσετε πρόσβαση λογαριασμών τοπικών συνεργατών σε πόρους cloud χρησιμοποιώντας τη συνεργασία Azure AD B2B.](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud)