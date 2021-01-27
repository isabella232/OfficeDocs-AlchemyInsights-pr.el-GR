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
ms.openlocfilehash: 4df9a98644f6bc7a30f9009719c5198db591afc9
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014800"
---
# <a name="delete-or-restore-applications"></a>Διαγραφή ή επαναφορά εφαρμογών

**Για να διαγράψετε μια εφαρμογή από τον μισθωτή σας Azure AD**:

1. Στην **πύλη Azure AD**, επιλέξτε **εταιρικές εφαρμογές**. Στη συνέχεια, εντοπίστε και επιλέξτε την εφαρμογή που θέλετε να διαγράψετε.
2. Στην ενότητα **Manage** στο αριστερό τμήμα του παραθύρου, επιλέξτε **Ιδιότητες**.
3. Επιλέξτε **Διαγραφή** και, στη συνέχεια, επιλέξτε **Ναι** για να επιβεβαιώσετε ότι θέλετε να διαγράψετε την εφαρμογή από τον μισθωτή σας Azure AD.

Για περισσότερες πληροφορίες σχετικά με τον τρόπο διαγραφής μιας εφαρμογής, ανατρέξτε στο θέμα [Γρήγορη εκκίνηση: Διαγραφή μιας εφαρμογής από τον μισθωτή του Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).

Στο PowerShell, το cmdlet [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) καταργεί τις ρυθμίσεις παραμέτρων του διακομιστή μεσολάβησης εφαρμογής από μια συγκεκριμένη εφαρμογή στο Azure Active Directory και μπορεί να διαγράψει πλήρως την εφαρμογή εάν έχει καθοριστεί.

Μπορείτε να **επαναφέρετε μια διαγραμμένη εφαρμογή χρησιμοποιώντας το** PowerShell. Αφού εντοπιστεί η εφαρμογή που θέλετε να επαναφέρετε, μπορείτε να την επαναφέρετε χρησιμοποιώντας την [Επαναφορά-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).
