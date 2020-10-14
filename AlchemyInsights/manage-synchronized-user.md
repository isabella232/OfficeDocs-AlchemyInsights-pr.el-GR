---
title: Διαχείριση συγχρονισμένου χρήστη
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: 7bf7d3f00308ff6bc973cd52e09ca51c5fd0f45b
ms.sourcegitcommit: 1fb324fd156008e77b7e2008af4b3dc1c0d0ea3e
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 10/13/2020
ms.locfileid: "48451400"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a><span data-ttu-id="d5b42-102">Δεν είναι δυνατός ο καθορισμός κύριας διεύθυνσης ηλεκτρονικού ταχυδρομείου, η αλλαγή χαρακτηριστικών χρήστη ή η κατάργηση/διαγραφή συγχρονισμένου χρήστη</span><span class="sxs-lookup"><span data-stu-id="d5b42-102">Unable to set primary email address, change user attributes, or remove/delete a synchronized user</span></span>

<span data-ttu-id="d5b42-103">Εάν ο συγχρονισμός καταλόγου είναι ενεργοποιημένος για το περιβάλλον σας, ορισμένα χαρακτηριστικά χρήστη ή αντικειμένου δεν μπορούν να αλλάξουν χρησιμοποιώντας το κέντρο διαχείρισης του Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="d5b42-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="d5b42-104">Για να διαχειριστείτε πλήρως τους συγχρονισμένους χρήστες και όλα τα χαρακτηριστικά τους, χρησιμοποιήστε την τοπική κονσόλα διαχείρισης χρηστών και ομάδων της υπηρεσίας καταλόγου Active Directory (ADSIEdit. msc).</span><span class="sxs-lookup"><span data-stu-id="d5b42-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="d5b42-105">Εναλλακτικά, μπορείτε να αλλάξετε μεμονωμένους χρήστες ή χαρακτηριστικά για συγχρονισμένους χρήστες που χρησιμοποιούν το PowerShell, όπως φαίνεται σε αυτά τα συνηθισμένα παραδείγματα:</span><span class="sxs-lookup"><span data-stu-id="d5b42-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span>

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
