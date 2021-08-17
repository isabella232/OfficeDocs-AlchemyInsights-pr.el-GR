---
title: Διαγραφή ή επαναφορά εφαρμογών
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
- "9004335"
- "7737"
ms.openlocfilehash: 0c7be98650ca87f36b66f0bb38fb665fc81525b7f3410da14b99fb67468c1e73
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54102571"
---
# <a name="delete-or-restore-applications"></a>Διαγραφή ή επαναφορά εφαρμογών

**Για να διαγράψετε μια εφαρμογή από το μισθωτή Azure AD:**

1. Στην πύλη **Azure AD, επιλέξτε** **μεγάλες εφαρμογές.** Στη συνέχεια, βρείτε και επιλέξτε την εφαρμογή που θέλετε να διαγράψετε.
2. Στην ενότητα **"Διαχείριση"** στο αριστερό τμήμα παραθύρου, επιλέξτε **"Ιδιότητες".**
3. Επιλέξτε **"Διαγραφή"** και, στη συνέχεια, **επιλέξτε "Ναι"** για να επιβεβαιώσετε ότι θέλετε να διαγράψετε την εφαρμογή από το μισθωτή Azure AD.

Για περισσότερες πληροφορίες σχετικά με τον τρόπο διαγραφής μιας εφαρμογής, ανατρέξτε στο θέμα Γρήγορη εκκίνηση: Διαγραφή εφαρμογής από [το μισθωτή Azure Active Directory (Azure AD).](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant)

Στο PowerShell, το [cmdlet Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) καταργεί τις ρυθμίσεις παραμέτρων διακομιστή μεσολάβησης εφαρμογών από μια συγκεκριμένη εφαρμογή στο Azure Active Directory και μπορεί να διαγράψει πλήρως την εφαρμογή, εάν καθοριστεί.

Μπορείτε να **επαναφέρετε μια διαγραμμένη εφαρμογή χρησιμοποιώντας** το PowerShell. Αφού προσδιοριστεί η εφαρμογή που θέλετε να επαναφέρετε, μπορείτε να την επαναφέρετε χρησιμοποιώντας [το Restore-AzureADDeletedApplication.](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)
