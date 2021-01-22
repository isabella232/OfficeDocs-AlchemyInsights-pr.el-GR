---
title: Ενεργοποίηση τεχνολογίας NDI
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004403"
- "7947"
ms.openlocfilehash: ea694898baffa50fca71957175eba3664dece44e
ms.sourcegitcommit: 112f18dce8257b98fab32d44910ee879efb44cb8
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935101"
---
# <a name="turn-on-ndi-technology"></a><span data-ttu-id="fe9a1-102">Ενεργοποίηση τεχνολογίας NDI</span><span class="sxs-lookup"><span data-stu-id="fe9a1-102">Turn on NDI technology</span></span>

<span data-ttu-id="fe9a1-103">Η τεχνολογία NDI απαιτεί δύο βήματα για να ενεργοποιηθεί για ένα χρήστη:</span><span class="sxs-lookup"><span data-stu-id="fe9a1-103">NDI technology requires two steps to be turned on for a user:</span></span>

1. <span data-ttu-id="fe9a1-104">Ο διαχειριστής μισθωτή πρέπει να ενεργοποιήσει την ιδιότητα "AllowNDIStreaming" στο CsTeamsMeetingPolicy.</span><span class="sxs-lookup"><span data-stu-id="fe9a1-104">The tenant admin must enable the 'AllowNDIStreaming' property in CsTeamsMeetingPolicy.</span></span>

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. <span data-ttu-id="fe9a1-105">Αφού συμπληρωθεί αυτή η αλλαγή, ο τελικός χρήστης πρέπει να ® NDI για το συγκεκριμένο πρόγραμμα-πελάτη από τις **Ρυθμίσεις > δικαιώματα.**</span><span class="sxs-lookup"><span data-stu-id="fe9a1-105">After this change has populated, the end user must turn on NDI® technology for their specific client from **Settings > Permissions**.</span></span>

<span data-ttu-id="fe9a1-106">Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα "Χρήση της τεχνολογίας NDI στο Microsoft Teams".](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings)</span><span class="sxs-lookup"><span data-stu-id="fe9a1-106">For more information, see [Use NDI technology in Microsoft Teams](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings).</span></span>
