---
title: Απαίτηση ισχυρού κωδικού πρόσβασης αλλαγή
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: f8790a26ec7c5de57f5dbfc9e1c162767c599f03
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36518759"
---
# <a name="change-strong-password-requirement"></a>Απαίτηση ισχυρού κωδικού πρόσβασης αλλαγή

Η Microsoft απαιτεί ισχυρούς κωδικούς πρόσβασης από προεπιλογή. 

Χρησιμοποιώντας PowerShell, μπορείτε να απενεργοποιήσετε ισχυρούς κωδικούς πρόσβασης για συγκεκριμένους χρήστες με αυτήν την εντολή:<br>
*Σύνολο MsolUser – UserPrincipalName <UserPrincipalName> – StrongPasswordRequired $false*

- [Περισσότερες πληροφορίες σχετικά με την πολιτική κωδικών πρόσβασης](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Τον τρόπο σύνδεσης στο Office 365 με PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Περισσότερες πληροφορίες σχετικά με τις εντολές PowerShell MsolUser](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)