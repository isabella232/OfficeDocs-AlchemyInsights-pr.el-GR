---
title: Ηλεκτρονική PowerShell του SharePoint
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 9/18/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 00ec337ce34da9d3c3fba0a71602c3078a556552
ms.sourcegitcommit: 6b102e079a7d30298105fd811a67efb707d6d5bf
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/23/2019
ms.locfileid: "37122999"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="6424b-102">Ηλεκτρονική PowerShell του SharePoint</span><span class="sxs-lookup"><span data-stu-id="6424b-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="6424b-103">Εργασία με PowerShell ή δέσμες ενεργειών εντός του SharePoint Online;</span><span class="sxs-lookup"><span data-stu-id="6424b-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="6424b-104">Για περισσότερες πληροφορίες, επισκεφτείτε τους παρακάτω συνδέσμους.</span><span class="sxs-lookup"><span data-stu-id="6424b-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="6424b-105">Γρήγορα αποτελέσματα με το κέλυφος διαχείρισης SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="6424b-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="6424b-106">Συνδεθείτε με το ΜFA PowerShell με έλεγχο ταυτότητας πολλαπλών παραγόντων (ΣΠΙ)</span><span class="sxs-lookup"><span data-stu-id="6424b-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="6424b-107">[Μοτίβα και πρακτικές του SharePoint (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) περιέχει μια βιβλιοθήκη των εντολών PowerShell που σας επιτρέπει να εκτελέσετε σύνθετες ενέργειες διαχείρισης προς το</span><span class="sxs-lookup"><span data-stu-id="6424b-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="6424b-108">Εάν αντιμετωπίζετε προβλήματα με τη σύνδεση με το κέλυφος διαχείρισης Μmt, βεβαιωθείτε ότι έχετε ενημερωθεί στην πιο πρόσφατη έκδοση και προσπαθήστε να [εισαγάγετε εκ νέου τη λειτουργική μονάδα](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) χρησιμοποιώντας *"εισαγωγή-λειτουργική μονάδα Microsoft. online. SharePoint. PowerShell".*</span><span class="sxs-lookup"><span data-stu-id="6424b-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="6424b-109">Εάν προσπαθείτε να εκτελέσετε δέσμες ενεργειών μοντέλου αντικειμένου-πελάτη, θα πρέπει να έχετε εγκατεστημένο στον τοπικό σας υπολογιστή το [SharePoint Online προγράμματα-πελάτες Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) .</span><span class="sxs-lookup"><span data-stu-id="6424b-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="6424b-110">Εάν αντιμετωπίζετε προβλήματα με την εκτέλεση δεσμών ενεργειών από PowerShell, ίσως θέλετε να εξετάσετε την εκτέλεση του PowerShell ως διαχειριστής και την αλλαγή της [πολιτικής εκτέλεσης](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span><span class="sxs-lookup"><span data-stu-id="6424b-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>