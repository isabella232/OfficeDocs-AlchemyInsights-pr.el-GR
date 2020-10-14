---
title: Αλλαγή διεύθυνσης ηλεκτρονικού ταχυδρομείου της ομάδας Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: f54ca5df09d0604f6d58c6c8a41dc907485e1f04
ms.sourcegitcommit: beb9715ac0c8e8333fef6764ecd346b7401a2612
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 10/10/2020
ms.locfileid: "48461833"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="d4eff-102">Αλλαγή διεύθυνσης ηλεκτρονικού ταχυδρομείου μιας ομάδας του Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="d4eff-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="d4eff-103">Μπορείτε να αλλάξετε τη διεύθυνση ηλεκτρονικού ταχυδρομείου μιας ομάδας του Microsoft 365 χρησιμοποιώντας το κέντρο διαχείρισης.</span><span class="sxs-lookup"><span data-stu-id="d4eff-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="d4eff-104">Απλώς επιλέξτε την ομάδα και επιλέξτε @edit διεύθυνση ηλεκτρονικού ταχυδρομείου.</span><span class="sxs-lookup"><span data-stu-id="d4eff-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="d4eff-105">Μπορείτε επίσης να χρησιμοποιήσετε την εντολή "εξω PowerShell" για να αλλάξετε την κύρια διεύθυνση SMTP μιας ομάδας του Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="d4eff-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

<span data-ttu-id="d4eff-106">Παράδειγμα</span><span class="sxs-lookup"><span data-stu-id="d4eff-106">Example:</span></span>

`et-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
