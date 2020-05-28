---
title: Διαχείριση συγχρονισμένου χρήστη
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: 84e337a7224fdd3c3ab7ad0f61240692fe007d5a
ms.sourcegitcommit: 82af227ac6d075e748e27c4ce6bdcf56628559cb
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 05/28/2020
ms.locfileid: "44407350"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a><span data-ttu-id="8cff9-102">Δεν είναι δυνατός ο ορισμός κύριας διεύθυνσης ηλεκτρονικού ταχυδρομείου, η αλλαγή χαρακτηριστικών χρήστη ή η κατάργηση/διαγραφή συγχρονισμένου χρήστη</span><span class="sxs-lookup"><span data-stu-id="8cff9-102">Unable to set primary email address, change user attributes, or remove/delete a synchronized user</span></span>

<span data-ttu-id="8cff9-103">Εάν είναι ενεργοποιημένος ο συγχρονισμός καταλόγου για το περιβάλλον σας, ορισμένα χαρακτηριστικά χρήστη ή αντικειμένου δεν μπορούν να αλλάξουν χρησιμοποιώντας το κέντρο διαχείρισης του Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="8cff9-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="8cff9-104">Για να διαχειριστείτε πλήρως τους συγχρονισμένους χρήστες και όλα τα χαρακτηριστικά τους, χρησιμοποιήστε τους τοπικούς χρήστες της υπηρεσίας καταλόγου Active Directory και την κονσόλα διαχείρισης ομάδων (adsiedit.msc).</span><span class="sxs-lookup"><span data-stu-id="8cff9-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="8cff9-105">Εναλλακτικά, μπορείτε να αλλάξετε μεμονωμένους χρήστες ή χαρακτηριστικά για συγχρονισμένους χρήστες χρησιμοποιώντας το powershell, όπως φαίνεται σε αυτά τα κοινά παραδείγματα:</span><span class="sxs-lookup"><span data-stu-id="8cff9-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- `Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

- `Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

- `Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
