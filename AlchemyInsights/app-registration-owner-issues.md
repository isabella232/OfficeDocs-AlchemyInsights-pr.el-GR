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
# <a name="app-registration-owner-issues"></a>Προβλήματα κατόχου καταχώρησης εφαρμογών

Ακολουθούν οι διαθέσιμες μέθοδοι για την προσθήκη εντολών ως κατόχων για εγγραφές εφαρμογών:

- Χρήση της λειτουργικής μονάδας Azure AD PowerShell -

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    Αναφορά: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)
- Χρήση του Azure CLI - `az ad app owner add`

    Αναφορά: [κάτοχος εφαρμογής διαφημίσεων az](https://docs.microsoft.com/cli/azure/ad/app/owner)
- Χρήση του MS Graph -

    Αναφορά: [Προσθήκη κατόχου - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)
- Χρήση της πύλης Azure AD - Μεταβείτε στο [portal.azure.com](https://portal.azure.com/) > Azure Active Directory > Καταχώρηση εφαρμογής > Επιλέξτε την εφαρμογή σας > Κάτοχοι > Προσθήκη κατόχων

**Δεν μπορείτε να προβάλετε την εφαρμογή σας στο App Registrations Blade, παρόλο που είστε ο κάτοχος αυτής της εφαρμογής;**

Ο κάτοχος μιας εφαρμογής δεν είναι διαχειριστικός ρόλος. Εάν η ρύθμιση ["Περιορισμός πρόσβασης στην πύλη](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) διαχείρισης Azure AD" είναι ενεργοποιημένη, τότε μόνο ο διαχειριστής θα μπορεί να δει τις εφαρμογές στην πύλη καταχώρησης εφαρμογών. Για να μπορεί ένας κάτοχος να δει τις εφαρμογές, είτε απενεργοποιήστε αυτήν τη ρύθμιση (Ορίστε αυτήν τη ρύθμιση σε NO) είτε εκχωρήστε ρόλο διαχειριστή στον κάτοχο μόνο για τη συγκεκριμένη εφαρμογή. Ωστόσο, για αυτό, θα χρειαστείτε μια άδεια χρήσης Του Azure AD Premium P2 και θα ενεργοποιήσετε τη [Διαχείριση προνομιακών ταυτοτήτων.](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)
