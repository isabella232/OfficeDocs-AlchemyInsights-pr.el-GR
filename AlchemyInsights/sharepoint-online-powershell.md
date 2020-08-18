---
title: PowerShell του SharePoint Online
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 300c07e7f0010eae2bd4fe893ece9d09aab93ba5
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/17/2020
ms.locfileid: "46786889"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="6788e-102">PowerShell του SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="6788e-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="6788e-103">Εργασία με PowerShell ή δέσμες ενεργειών εντός του SharePoint Online;</span><span class="sxs-lookup"><span data-stu-id="6788e-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="6788e-104">Επισκεφθείτε τις παρακάτω συνδέσεις για περισσότερες πληροφορίες.</span><span class="sxs-lookup"><span data-stu-id="6788e-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="6788e-105">Γρήγορα αποτελέσματα με το κέλυφος διαχείρισης του SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="6788e-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="6788e-106">Σύνδεση με το SPO PowerShell με έλεγχο ταυτότητας πολλών παραγόντων (ΣΠΙ)</span><span class="sxs-lookup"><span data-stu-id="6788e-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="6788e-107">Τα [μοτίβα και οι πρακτικές του SharePoint (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) περιέχουν μια βιβλιοθήκη εντολών του PowerShell που σας επιτρέπει να εκτελείτε σύνθετες ενέργειες διαχείρισης προς το SPO.</span><span class="sxs-lookup"><span data-stu-id="6788e-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="6788e-108">Εάν αντιμετωπίζετε προβλήματα κατά τη σύνδεση με το κέλυφος διαχείρισης SPO, βεβαιωθείτε ότι έχετε ενημερώσει την πιο πρόσφατη έκδοση και προσπαθήστε να [επαναλάβετε την εισαγωγή της λειτουργικής μονάδας χρησιμοποιώντας τη](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) φράση *"εισαγωγή-λειτουργική μονάδα Microsoft. online. SharePoint. PowerShell".*</span><span class="sxs-lookup"><span data-stu-id="6788e-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="6788e-109">Εάν προσπαθείτε να εκτελέσετε δέσμες ενεργειών μοντέλου αντικειμένου από την πλευρά του προγράμματος-πελάτη, θα πρέπει να έχετε εγκαταστήσει το [SDK στοιχεία προγράμματος-πελάτη του SharePoint Online](https://www.microsoft.com/download/details.aspx?id=42038) στον τοπικό υπολογιστή σας.</span><span class="sxs-lookup"><span data-stu-id="6788e-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="6788e-110">Εάν αντιμετωπίζετε προβλήματα με την εκτέλεση δεσμών ενεργειών από το PowerShell, μπορεί να θέλετε να εξετάσετε την εκτέλεση του PowerShell ως διαχειριστή και να αλλάξετε την [πολιτική εκτέλεσης](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span><span class="sxs-lookup"><span data-stu-id="6788e-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>