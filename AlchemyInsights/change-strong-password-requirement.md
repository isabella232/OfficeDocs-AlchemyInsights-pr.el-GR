---
title: Αλλαγή απαίτησης ισχυρού κωδικού πρόσβασης
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
ms.openlocfilehash: a054735a0c139c90d76098297bb9984d37464d3b
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706561"
---
# <a name="change-strong-password-requirement"></a>Αλλαγή απαίτησης ισχυρού κωδικού πρόσβασης

Η Microsoft απαιτεί ισχυρούς κωδικούς πρόσβασης από προεπιλογή. 

Χρησιμοποιώντας το PowerShell, μπορείτε να απενεργοποιήσετε ισχυρούς κωδικούς πρόσβασης για συγκεκριμένους χρήστες με αυτήν την εντολή:<br>
*Set-MsolUser –Όνομα <UserPrincipalName> εγγραφής χρήστη –Ισχυρός κωδικός πρόσβασης Απαιτείται $false*

- [Περισσότερες πληροφορίες σχετικά με την πολιτική κωδικού πρόσβασης](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Τρόπος σύνδεσης στο Microsoft 365 με το PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Περισσότερες πληροφορίες σχετικά με τις εντολές PowerShell MsolUser](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
