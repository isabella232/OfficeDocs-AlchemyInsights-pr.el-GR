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
ms.openlocfilehash: 21f80a7cc8b00ac56acdb05add1e1bfdfac9d827
ms.sourcegitcommit: c061f1dfa6f557a9ec083dd030b73b121d9864ea
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43286263"
---
# <a name="change-strong-password-requirement"></a>Αλλαγή απαίτησης ισχυρού κωδικού πρόσβασης

Η Microsoft απαιτεί ισχυρούς κωδικούς πρόσβασης από προεπιλογή. 

Χρησιμοποιώντας το PowerShell, μπορείτε να απενεργοποιήσετε ισχυρούς κωδικούς πρόσβασης για συγκεκριμένους χρήστες με αυτήν την εντολή:<br>
*Set-MsolUser –Όνομα <UserPrincipalName> εγγραφής χρήστη –Ισχυρός κωδικός πρόσβασης Απαιτείται $false*

- [Περισσότερες πληροφορίες σχετικά με την πολιτική κωδικού πρόσβασης](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Τρόπος σύνδεσης στο Office 365 με το PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Περισσότερες πληροφορίες σχετικά με τις εντολές PowerShell MsolUser](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
- [Ορισμός κωδικού πρόσβασης μεμονωμένου χρήστη που δεν λήγει ποτέ](https://docs.microsoft.com/microsoft-365/admin/add-users/set-password-to-never-expire)
