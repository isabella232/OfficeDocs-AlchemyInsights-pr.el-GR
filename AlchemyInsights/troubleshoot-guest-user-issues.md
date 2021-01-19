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
ms.openlocfilehash: 0f2a10b918fee067b167ab58ac2544a89e0c8ea1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901167"
---
# <a name="troubleshoot-guest-user-issues"></a>Αντιμετώπιση προβλημάτων χρήστη επισκέπτη

1. Για οδηγίες σχετικά με τη διαχείριση της πρόσβασης επισκεπτών σε εφαρμογές, ανατρέξτε στο θέμα [Διαχείριση πρόσβασης επισκέπτη με σχόλια Azure AD Access](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews).
1. [Προσθήκη προσκεκλημένων χρηστών στον κατάλογό σας στην πύλη Azure](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal): σε αυτήν την γρήγορη εκκίνηση, θα προσθέσετε έναν νέο χρήστη επισκέπτη στον κατάλογο Azure AD μέσω της πύλης Azure, θα στείλετε μια πρόσκληση και θα δείτε ποια είναι η διαδικασία εξαργύρωσης της πρόσκλησης του χρήστη επισκέπτη.
1. [Προσθήκη χρήστη επισκέπτη με το PowerShell](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell): σε αυτήν την γρήγορη εκκίνηση, θα χρησιμοποιήσετε την εντολή New-AzureADMSInvitation για να προσθέσετε έναν χρήστη επισκέπτη στον μισθωτή σας Azure.
1. Για να μάθετε πώς μπορείτε να αντιστοιχίσετε χρήστες και ομάδες σε εταιρικές εφαρμογές στο Azure Active Directory (Azure AD), είτε μέσα από την πύλη Azure είτε χρησιμοποιώντας το PowerShell, ανατρέξτε στο θέμα [Διαχείριση ανάθεσης χρήστη για μια εφαρμογή στο Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal). 
1. Η συνεργασία B2B του Azure Active Directory (Azure AD) συνεργάζεται με τις περισσότερες εφαρμογές που ενσωματώνονται με το Azure AD. Σε αυτό το [άρθρο](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps), θα περπατήσουμε μέσα σε οδηγίες για τη ρύθμιση ορισμένων δημοφιλών εφαρμογών SaaS για χρήση με το Azure AD B2B.
1. Ως οργανισμός που χρησιμοποιεί δυνατότητες συνεργασίας B2B υπηρεσίας καταλόγου Active Directory (Azure AD) για να προσκαλεί τους χρήστες των συνεργατών σας στο Azure AD, μπορείτε πλέον να παρέχετε σε αυτούς τους χρήστες B2B πρόσβαση σε εφαρμογές εσωτερικής εγκατάστασης. Αυτές οι εφαρμογές εσωτερικής εγκατάστασης μπορούν να χρησιμοποιούν έλεγχο ταυτότητας που βασίζεται στο SAML ή ενσωματωμένο έλεγχο ταυτότητας των Windows (IWA) με αντιπροσώπευση Kerberos περιορισμένη (KCD). Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα Εκχώρηση χρηστών B2B στο Azure AD για πρόσβαση στις εφαρμογές εσωτερικής εγκατάστασης](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises).
1. Μάθετε πώς μπορείτε να [εκχωρήσετε πρόσβαση σε λογαριασμούς συνεργατών με τοπική διαχείριση σε πόρους του cloud χρησιμοποιώντας τη συνεργασία του Azure AD B2B](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud).