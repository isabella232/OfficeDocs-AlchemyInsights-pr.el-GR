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
ms.openlocfilehash: a943c59d67c512e6326856dacd0053db121f6aa3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36541990"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a><span data-ttu-id="e7358-102">Δεν είναι δυνατό να ορίσετε την κύρια διεύθυνση ηλεκτρονικού ταχυδρομείου ή να αλλάξετε τα χαρακτηριστικά χρήστη</span><span class="sxs-lookup"><span data-stu-id="e7358-102">Unable to set primary email address or change user attributes</span></span>

<span data-ttu-id="e7358-103">Εάν είναι ενεργοποιημένη η συγχρονισμού καταλόγου για το περιβάλλον σας, ορισμένα χαρακτηριστικά του χρήστη ή το αντικείμενο δεν μπορεί να αλλάξει χρησιμοποιώντας το Κέντρο διαχείρισης Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="e7358-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="e7358-104">Για να διαχειρίζονται πλήρως συγχρονισμένη χρήστες και όλα τα χαρακτηριστικά τους, χρησιμοποιήσετε την τοπική υπηρεσία καταλόγου active directory χρήστες και ομάδες Κονσόλα διαχείρισης (adsiedit.msc).</span><span class="sxs-lookup"><span data-stu-id="e7358-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="e7358-105">Εναλλακτικά, μπορείτε να αλλάξετε μεμονωμένους χρήστες ή χαρακτηριστικών για συγχρονισμένες χρήστες χρησιμοποιώντας powershell, όπως φαίνεται σε αυτά τα κοινά παραδείγματα:</span><span class="sxs-lookup"><span data-stu-id="e7358-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- <span data-ttu-id="e7358-106">Σύνολο MsolUser - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="e7358-106">Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span></span>
- <span data-ttu-id="e7358-107">Σύνολο-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com" - DisplayName "Δοκιμής χρήστη" - Επώνυμο "Χρήστης"-τον τίτλο "Διευθυντής"-τμήμα "HR"</span><span class="sxs-lookup"><span data-stu-id="e7358-107">Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"</span></span>
- <span data-ttu-id="e7358-108">Κατάργηση-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="e7358-108">Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com</span></span>