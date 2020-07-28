---
title: Δεν είναι δυνατή η αλλαγή του ονόματος χρήστη
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 34aecdf503699ee500179f0958158fc964d77fcb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439553"
---
# <a name="unable-to-change-username"></a><span data-ttu-id="04acb-102">Δεν είναι δυνατή η αλλαγή του ονόματος χρήστη</span><span class="sxs-lookup"><span data-stu-id="04acb-102">Unable to change UserName</span></span>

<span data-ttu-id="04acb-103">Σε ορισμένες περιπτώσεις, οι αλλαγές UPN (UserPrincipalName) δεν μεταδίδονται στο cloud.</span><span class="sxs-lookup"><span data-stu-id="04acb-103">In some cases, UPN (UserPrincipalName) changes aren't propagated to the cloud.</span></span> <span data-ttu-id="04acb-104">Ενδέχεται να λάβετε σφάλματα επικύρωσης στην πύλη του Office 365 ή να μην μπορείτε να αλλάξετε το όνομα χρήστη ή τη διεύθυνση ηλεκτρονικού ταχυδρομείου.</span><span class="sxs-lookup"><span data-stu-id="04acb-104">You might receive validation errors in the Office 365 portal or be unable to change the username or email address.</span></span> <span data-ttu-id="04acb-105">Για να επιλύσετε αυτό το ζήτημα, ορίστε με μη αυτόματο τρόπο το UserPrincipalName χρησιμοποιώντας αυτήν την εντολή PowerShell.</span><span class="sxs-lookup"><span data-stu-id="04acb-105">To resolve this issue, manually set UserPrincipalName using this PowerShell command.</span></span>

<span data-ttu-id="04acb-106">**Παράδειγμα: Μετονομασία χρήστη**</span><span class="sxs-lookup"><span data-stu-id="04acb-106">**Example: Rename a user**</span></span>

<span data-ttu-id="04acb-107">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="04acb-107">PowerShellCopy</span></span>

<span data-ttu-id="04acb-108">PS C: \> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span><span class="sxs-lookup"><span data-stu-id="04acb-108">PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span></span>

<span data-ttu-id="04acb-109">Αυτή η εντολή μετονομάζει davidc@contoso.com σε davidchew@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="04acb-109">This command renames davidc@contoso.com to davidchew@contoso.com.</span></span>

<span data-ttu-id="04acb-110">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span><span class="sxs-lookup"><span data-stu-id="04acb-110">For more information, see [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span></span>