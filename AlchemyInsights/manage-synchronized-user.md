---
title: Διαχείριση χρήστη συγχρονίζονται
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
ms.openlocfilehash: 5a383bdd17c5fa055c35a923ca36e0e0f6d429e4
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35380505"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a><span data-ttu-id="cc1d2-102">Δεν είναι δυνατό να ορίσετε την κύρια διεύθυνση ηλεκτρονικού ταχυδρομείου ή να αλλάξετε τα χαρακτηριστικά χρήστη</span><span class="sxs-lookup"><span data-stu-id="cc1d2-102">Unable to set primary email address or change user attributes</span></span>

<span data-ttu-id="cc1d2-103">Εάν είναι ενεργοποιημένη η συγχρονισμού καταλόγου για το περιβάλλον σας ορισμένα χαρακτηριστικά χρήστης ή το αντικείμενο δεν μπορεί να αλλάξει χρησιμοποιώντας το Κέντρο διαχείρισης.</span><span class="sxs-lookup"><span data-stu-id="cc1d2-103">If directory synchronization is enabled for your environment some user or object attributes cannot be changed using the Admin Center.</span></span>
<span data-ttu-id="cc1d2-104">Για να διαχειρίζονται πλήρως συγχρονισμένη χρήστες και όλα τα χαρακτηριστικά τους, χρησιμοποιήσετε την τοπική υπηρεσία καταλόγου active directory χρήστες και ομάδες Κονσόλα διαχείρισης (adsiedit.msc).</span><span class="sxs-lookup"><span data-stu-id="cc1d2-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="cc1d2-105">Εναλλακτικά, μπορείτε να αλλάξετε μεμονωμένους χρήστες ή χαρακτηριστικών για συγχρονισμένες χρήστες χρησιμοποιώντας powershell, όπως φαίνεται σε αυτά τα κοινά παραδείγματα:</span><span class="sxs-lookup"><span data-stu-id="cc1d2-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- <span data-ttu-id="cc1d2-106">Σύνολο MsolUser - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="cc1d2-106">Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span></span>
- <span data-ttu-id="cc1d2-107">Σύνολο-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com" - DisplayName "Δοκιμής χρήστη" - Επώνυμο "Χρήστης"-τον τίτλο "Διευθυντής"-τμήμα "HR"</span><span class="sxs-lookup"><span data-stu-id="cc1d2-107">Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"</span></span>
- <span data-ttu-id="cc1d2-108">Κατάργηση-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="cc1d2-108">Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com</span></span>