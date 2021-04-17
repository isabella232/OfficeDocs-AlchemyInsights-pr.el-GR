---
title: Sharepoint Online PowerShell
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 839a70282b4dd619e9dbe8167ef0e409e468b1ad
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830582"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="7bfab-102">Sharepoint Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="7bfab-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="7bfab-103">Εργάζεστε με το PowerShell ή δέσμες ενεργειών μέσα στο Sharepoint Online;</span><span class="sxs-lookup"><span data-stu-id="7bfab-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="7bfab-104">Για περισσότερες πληροφορίες, επισκεφθείτε τις παρακάτω συνδέσεις.</span><span class="sxs-lookup"><span data-stu-id="7bfab-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="7bfab-105">Γρήγορα αποτελέσματα με το Κέλυφος διαχείρισης του SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="7bfab-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="7bfab-106">Σύνδεση στο SPO PowerShell με έλεγχο ταυτότητας πολλών παραγόντων (MFA)</span><span class="sxs-lookup"><span data-stu-id="7bfab-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="7bfab-107">[Τα μοτίβα και οι πρακτικές του SharePoint (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) περιέχουν μια βιβλιοθήκη εντολών του PowerShell που σας επιτρέπει να εκτελείτε σύνθετες ενέργειες διαχείρισης προς το SPO.</span><span class="sxs-lookup"><span data-stu-id="7bfab-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="7bfab-108">Εάν αντιμετωπίζετε προβλήματα σύνδεσης με το κέλυφος διαχείρισης SPO, βεβαιωθείτε ότι έχετε [](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) ενημερώσει την πιο πρόσφατη έκδοση και προσπαθήστε να εισαγάγετε ξανά τη λειτουργική μονάδα χρησιμοποιώντας *τη "Εισαγωγή λειτουργικής μονάδας Microsoft.Online.SharePoint.PowerShell".*</span><span class="sxs-lookup"><span data-stu-id="7bfab-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="7bfab-109">Εάν προσπαθείτε να εκτελέσετε δέσμες ενεργειών μοντέλου αντικειμένου από την πλευρά του προγράμματος-πελάτη, θα πρέπει να έχετε εγκαταστήσει το SDK στοιχείων προγράμματος-πελάτη του [Sharepoint Online](https://www.microsoft.com/download/details.aspx?id=42038) στον τοπικό υπολογιστή σας.</span><span class="sxs-lookup"><span data-stu-id="7bfab-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="7bfab-110">Εάν αντιμετωπίζετε προβλήματα κατά την εκτέλεση δεσμών ενεργειών από το PowerShell, μπορείτε να εξετάσετε το ενδεχόμενο να εκτελείτε το PowerShell ως διαχειριστής και να αλλάξετε την [πολιτική εκτέλεσης.](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)</span><span class="sxs-lookup"><span data-stu-id="7bfab-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>