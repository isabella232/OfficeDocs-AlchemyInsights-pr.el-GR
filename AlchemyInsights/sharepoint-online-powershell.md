---
title: Ηλεκτρονικό PowerShell του Sharepoint
ms.author: v-todmc
author: todmccoy
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
ms.openlocfilehash: 8c270748fc75f929371fbb2856daad3ae61a1540
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764261"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="0f6a5-102">Ηλεκτρονικό PowerShell του Sharepoint</span><span class="sxs-lookup"><span data-stu-id="0f6a5-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="0f6a5-103">Εργασία με το PowerShell ή δέσμες ενεργειών στο Sharepoint Online;</span><span class="sxs-lookup"><span data-stu-id="0f6a5-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="0f6a5-104">Επισκεφθείτε τους παρακάτω συνδέσμους για περισσότερες πληροφορίες.</span><span class="sxs-lookup"><span data-stu-id="0f6a5-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="0f6a5-105">Γρήγορα αποτελέσματα με το κέλυφος διαχείρισης του SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="0f6a5-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="0f6a5-106">Σύνδεση στο SPO PowerShell με έλεγχο ταυτότητας πολλών παραγόντων (MFA)</span><span class="sxs-lookup"><span data-stu-id="0f6a5-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="0f6a5-107">[Τα μοτίβα και οι πρακτικές του SharePoint (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) περιέχουν μια βιβλιοθήκη εντολών PowerShell που σας επιτρέπει να εκτελείτε σύνθετες ενέργειες διαχείρισης προς το SPO.</span><span class="sxs-lookup"><span data-stu-id="0f6a5-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="0f6a5-108">Εάν αντιμετωπίζετε ζητήματα σύνδεσης με το κέλυφος διαχείρισης SPO, βεβαιωθείτε ότι έχετε ενημερωθεί στην πιο πρόσφατη έκδοση και προσπαθήστε να [εισαγάγετε ξανά τη λειτουργική μονάδα](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) *χρησιμοποιώντας την επιλογή "Εισαγωγή-λειτουργική μονάδα Microsoft.Online.SharePoint.PowerShell".*</span><span class="sxs-lookup"><span data-stu-id="0f6a5-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="0f6a5-109">Εάν προσπαθείτε να εκτελέσετε δέσμες ενεργειών μοντέλου αντικειμένου υπολογιστή-πελάτη, θα πρέπει να έχετε εγκαταστήσει το [SDK στοιχείων προγράμματος-πελάτη Sharepoint Online](https://www.microsoft.com/download/details.aspx?id=42038) στον τοπικό υπολογιστή σας.</span><span class="sxs-lookup"><span data-stu-id="0f6a5-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="0f6a5-110">Εάν αντιμετωπίζετε ζητήματα που εκτελούνται σε δέσμες ενεργειών από το PowerShell, ίσως θελήσετε να εξετάσετε το ενδεχόμενο να εκτελέσετε το PowerShell ως διαχειριστή και να αλλάξετε την [πολιτική εκτέλεσης](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span><span class="sxs-lookup"><span data-stu-id="0f6a5-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>