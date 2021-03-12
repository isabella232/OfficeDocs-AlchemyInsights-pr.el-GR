---
title: Sharepoint Online PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: b7580f0e609d21bdc13fc07fda0bfd15bdb7a7ca
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709070"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="aa966-102">Sharepoint Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="aa966-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="aa966-103">Εργάζεστε με το PowerShell ή με δέσμες ενεργειών στο Sharepoint Online;</span><span class="sxs-lookup"><span data-stu-id="aa966-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="aa966-104">Επισκεφτείτε τις παρακάτω συνδέσεις για περισσότερες πληροφορίες.</span><span class="sxs-lookup"><span data-stu-id="aa966-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="aa966-105">Γρήγορα αποτελέσματα με το Κέλυφος διαχείρισης του SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="aa966-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="aa966-106">Σύνδεση στο SPO PowerShell με έλεγχο ταυτότητας πολλών παραγόντων (MFA)</span><span class="sxs-lookup"><span data-stu-id="aa966-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="aa966-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span><span class="sxs-lookup"><span data-stu-id="aa966-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="aa966-108">Εάν αντιμετωπίζετε προβλήματα σύνδεσης με το κέλυφος διαχείρισης του SPO, βεβαιωθείτε ότι [](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) έχετε ενημερώσει την πιο πρόσφατη έκδοση και προσπαθήστε να εισαγάγετε ξανά τη λειτουργική μονάδα χρησιμοποιώντας τη *"Import-Module Microsoft.Online.SharePoint.PowerShell".*</span><span class="sxs-lookup"><span data-stu-id="aa966-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="aa966-109">Εάν προσπαθείτε να εκτελέσετε δέσμες ενεργειών μοντέλου αντικειμένου από την πλευρά του προγράμματος-πελάτη, θα πρέπει να έχετε το SDK στοιχείων προγράμματος-πελάτη του [Sharepoint Online](https://www.microsoft.com/download/details.aspx?id=42038) εγκατεστημένο στον τοπικό υπολογιστή σας.</span><span class="sxs-lookup"><span data-stu-id="aa966-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="aa966-110">Εάν αντιμετωπίζετε προβλήματα με την εκτέλεση δεσμών ενεργειών από το PowerShell, εξετάστε το ενδεχόμενο να εκτελείτε το PowerShell ως διαχειριστής και να αλλάξετε την [πολιτική εκτέλεσης.](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)</span><span class="sxs-lookup"><span data-stu-id="aa966-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>