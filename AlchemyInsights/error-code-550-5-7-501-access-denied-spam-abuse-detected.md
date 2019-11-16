---
title: Κωδικός σφάλματος 550 5.7.501 δεν επιτρέπεται η πρόσβαση, εντοπίστηκε κατάχρηση ανεπιθύμητης αλληλογραφίας
ms.author: chrisda
author: chrisda
ms.date: 6/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "351"
- "3100015"
ms.assetid: 3105905c-e7a0-42a7-9c5a-61dc56a1d6fc
ms.openlocfilehash: 545cab07cc7c49def849be20bb6363da228a5393
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 11/15/2019
ms.locfileid: "36740141"
---
# <a name="550-57501-access-denied-spam-abuse-detected"></a><span data-ttu-id="710c7-102">550 5.7.501 δεν επιτρέπεται η πρόσβαση, εντοπίστηκε κατάχρηση ανεπιθύμητης αλληλογραφίας</span><span class="sxs-lookup"><span data-stu-id="710c7-102">550 5.7.501 Access denied, spam abuse detected</span></span>

<span data-ttu-id="710c7-103">Συνήθως, αυτό το μήνυμα παρουσιάζεται όταν οι χρήστες στέλνουν μηνύματα ηλεκτρονικού ταχυδρομείου από διευθύνσεις IP χρησιμοποιώντας τον αρχικό τομέα *. onmicrosoft.com* που έχει αντιστοιχιστεί σε νέους ενοίκους στο Office 365.</span><span class="sxs-lookup"><span data-stu-id="710c7-103">Typically, this message occurs when users send email messages from IP addresses using the initial *.onmicrosoft.com* domain that's assigned to new tenants in Office 365.</span></span> <span data-ttu-id="710c7-104">Ο ευκολότερος τρόπος επίλυσης αυτού του προβλήματος είναι:</span><span class="sxs-lookup"><span data-stu-id="710c7-104">The easiest way to resolve this problem is to:</span></span>

1. <span data-ttu-id="710c7-105">[Προσθέστε έναν τομέα στον μισθωτή σας](https://docs.microsoft.com//office365/admin/setup/add-domain).</span><span class="sxs-lookup"><span data-stu-id="710c7-105">[Add a domain to your tenant](https://docs.microsoft.com//office365/admin/setup/add-domain).</span></span>

2. <span data-ttu-id="710c7-106">[Αλλάξτε την κύρια διεύθυνση ηλεκτρονικού ταχυδρομείου των χρηστών](https://docs.microsoft.com//office365/admin/add-users/change-a-user-name-and-email-address) σας στον νέο προσαρμοσμένο τομέα που μόλις προσθέσατε.</span><span class="sxs-lookup"><span data-stu-id="710c7-106">[Change your users' primary email address](https://docs.microsoft.com//office365/admin/add-users/change-a-user-name-and-email-address) to the new custom domain you just added.</span></span>
