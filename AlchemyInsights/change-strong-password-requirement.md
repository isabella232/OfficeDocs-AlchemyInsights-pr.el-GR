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
# <a name="change-strong-password-requirement"></a><span data-ttu-id="dd877-102">Αλλαγή απαίτησης ισχυρού κωδικού πρόσβασης</span><span class="sxs-lookup"><span data-stu-id="dd877-102">Change strong password requirement</span></span>

<span data-ttu-id="dd877-103">Η Microsoft απαιτεί ισχυρούς κωδικούς πρόσβασης από προεπιλογή.</span><span class="sxs-lookup"><span data-stu-id="dd877-103">Microsoft requires strong passwords by default.</span></span> 

<span data-ttu-id="dd877-104">Χρησιμοποιώντας το PowerShell, μπορείτε να απενεργοποιήσετε ισχυρούς κωδικούς πρόσβασης για συγκεκριμένους χρήστες με αυτήν την εντολή:</span><span class="sxs-lookup"><span data-stu-id="dd877-104">Using PowerShell, you can disable strong passwords for specific users with this command:</span></span><br>
<span data-ttu-id="dd877-105">*Set-MsolUser –Όνομα <UserPrincipalName> εγγραφής χρήστη –Ισχυρός κωδικός πρόσβασης Απαιτείται $false*</span><span class="sxs-lookup"><span data-stu-id="dd877-105">*Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false*</span></span>

- [<span data-ttu-id="dd877-106">Περισσότερες πληροφορίες σχετικά με την πολιτική κωδικού πρόσβασης</span><span class="sxs-lookup"><span data-stu-id="dd877-106">More information on password policy</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [<span data-ttu-id="dd877-107">Τρόπος σύνδεσης στο Microsoft 365 με το PowerShell</span><span class="sxs-lookup"><span data-stu-id="dd877-107">How to connect to Microsoft 365 with PowerShell</span></span>](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [<span data-ttu-id="dd877-108">Περισσότερες πληροφορίες σχετικά με τις εντολές PowerShell MsolUser</span><span class="sxs-lookup"><span data-stu-id="dd877-108">More information on PowerShell MsolUser commands</span></span>](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
