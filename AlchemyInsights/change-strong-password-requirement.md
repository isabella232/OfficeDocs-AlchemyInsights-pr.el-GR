---
title: Απαίτηση ισχυρού κωδικού πρόσβασης αλλαγή
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: 53affd2a347c004e7b21b353c2b3df98bc30a585
ms.sourcegitcommit: a7e5ca472000dfec471950bafd12eee8d7144f74
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35701584"
---
# <a name="change-strong-password-requirement"></a>Απαίτηση ισχυρού κωδικού πρόσβασης αλλαγή

Οι ισχυροί κωδικοί πρόσβασης απαιτούνται από προεπιλογή. 

Χρησιμοποιώντας PowerShell, μπορείτε να απενεργοποιήσετε ισχυρούς κωδικούς πρόσβασης για συγκεκριμένους χρήστες με αυτήν την εντολή:<br>
*Σύνολο MsolUser – UserPrincipalName <UserPrincipalName> – StrongPasswordRequired $false*

- [Περισσότερες πληροφορίες σχετικά με την πολιτική κωδικών πρόσβασης](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Πώς να συνδεθείτε σε O365 με PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Περισσότερες πληροφορίες σχετικά με τις εντολές PowerShell MsolUser](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)