---
title: Προβλήματα κατόχου καταχώρησης εφαρμογών
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9655"
ms.openlocfilehash: 9dc3b1d54bb263d5e53e02a4e4dadc8cf3c1e400
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404773"
---
# <a name="app-registration-owner-issues"></a><span data-ttu-id="fc12f-102">Προβλήματα κατόχου καταχώρησης εφαρμογών</span><span class="sxs-lookup"><span data-stu-id="fc12f-102">App Registration Owner issues</span></span>

<span data-ttu-id="fc12f-103">Ακολουθούν οι διαθέσιμες μέθοδοι για την προσθήκη εντολών ως κατόχων για εγγραφές εφαρμογών:</span><span class="sxs-lookup"><span data-stu-id="fc12f-103">Following are the available methods to add principals as owners for app registrations:</span></span>

- <span data-ttu-id="fc12f-104">Χρήση της λειτουργικής μονάδας Azure AD PowerShell -</span><span class="sxs-lookup"><span data-stu-id="fc12f-104">Using Azure AD PowerShell Module -</span></span>

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    <span data-ttu-id="fc12f-105">Αναφορά: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span><span class="sxs-lookup"><span data-stu-id="fc12f-105">Reference: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span></span>
- <span data-ttu-id="fc12f-106">Χρήση του Azure CLI - `az ad app owner add`</span><span class="sxs-lookup"><span data-stu-id="fc12f-106">Using Azure CLI - `az ad app owner add`</span></span>

    <span data-ttu-id="fc12f-107">Αναφορά: [κάτοχος εφαρμογής διαφημίσεων az](https://docs.microsoft.com/cli/azure/ad/app/owner)</span><span class="sxs-lookup"><span data-stu-id="fc12f-107">Reference: [az ad app owner](https://docs.microsoft.com/cli/azure/ad/app/owner)</span></span>
- <span data-ttu-id="fc12f-108">Χρήση του MS Graph -</span><span class="sxs-lookup"><span data-stu-id="fc12f-108">Using MS Graph -</span></span>

    <span data-ttu-id="fc12f-109">Αναφορά: [Προσθήκη κατόχου - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span><span class="sxs-lookup"><span data-stu-id="fc12f-109">Reference: [Add owner - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span></span>
- <span data-ttu-id="fc12f-110">Χρήση της πύλης Azure AD - Μεταβείτε στο [portal.azure.com](https://portal.azure.com/) > Azure Active Directory > Καταχώρηση εφαρμογής > Επιλέξτε την εφαρμογή σας > Κάτοχοι > Προσθήκη κατόχων</span><span class="sxs-lookup"><span data-stu-id="fc12f-110">Using the Azure AD Portal - Navigate to [portal.azure.com](https://portal.azure.com/) > Azure Active directory > App Registration > Select your application > Owners > Add Owners</span></span>

<span data-ttu-id="fc12f-111">**Δεν μπορείτε να προβάλετε την εφαρμογή σας στο App Registrations Blade, παρόλο που είστε ο κάτοχος αυτής της εφαρμογής;**</span><span class="sxs-lookup"><span data-stu-id="fc12f-111">**Cannot view your application on App Registrations blade even though you are the owner of that application?**</span></span>

<span data-ttu-id="fc12f-112">Ο κάτοχος μιας εφαρμογής δεν είναι διαχειριστικός ρόλος.</span><span class="sxs-lookup"><span data-stu-id="fc12f-112">Owner of an app is not an administrative role.</span></span> <span data-ttu-id="fc12f-113">Εάν η ρύθμιση ["Περιορισμός πρόσβασης στην πύλη](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) διαχείρισης Azure AD" είναι ενεργοποιημένη, τότε μόνο ο διαχειριστής θα μπορεί να δει τις εφαρμογές στην πύλη καταχώρησης εφαρμογών.</span><span class="sxs-lookup"><span data-stu-id="fc12f-113">If the setting [Restrict access to Azure AD administration portal](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) is enabled, then only admin will be able to view the applications on App Registration portal.</span></span> <span data-ttu-id="fc12f-114">Για να μπορεί ένας κάτοχος να δει τις εφαρμογές, είτε απενεργοποιήστε αυτήν τη ρύθμιση (Ορίστε αυτήν τη ρύθμιση σε NO) είτε εκχωρήστε ρόλο διαχειριστή στον κάτοχο μόνο για τη συγκεκριμένη εφαρμογή.</span><span class="sxs-lookup"><span data-stu-id="fc12f-114">For an owner to be able to view the applications, either disable this setting (Set this to NO) or assign admin role to the owner for only the specific application.</span></span> <span data-ttu-id="fc12f-115">Ωστόσο, για αυτό, θα χρειαστείτε μια άδεια χρήσης Του Azure AD Premium P2 και θα ενεργοποιήσετε τη [Διαχείριση προνομιακών ταυτοτήτων.](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)</span><span class="sxs-lookup"><span data-stu-id="fc12f-115">However for this, you will require an Azure AD Premium P2 license and enable [Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).</span></span>
