---
title: Αλλαγή απαίτησης ισχυρού κωδικού πρόσβασης
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: 8a82c002bd64a33556b632545e98355e860848d845e122bfea06fbc5ee5dcb90
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54070684"
---
# <a name="change-strong-password-requirement"></a>Αλλαγή απαίτησης ισχυρού κωδικού πρόσβασης

Η Microsoft απαιτεί ισχυρούς κωδικούς πρόσβασης από προεπιλογή.

Χρησιμοποιώντας το PowerShell, μπορείτε να απενεργοποιήσετε ισχυρούς κωδικούς πρόσβασης για συγκεκριμένους χρήστες με αυτές τις εντολές:

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

Για να απενεργοποιήσετε ισχυρούς κωδικούς πρόσβασης για όλους τους χρήστες, χρησιμοποιήστε:

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [Περισσότερες πληροφορίες σχετικά με την πολιτική κωδικών πρόσβασης](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Τρόπος σύνδεσης με Microsoft 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Περισσότερες πληροφορίες σχετικά με τις εντολές του PowerShell MsolUser](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
