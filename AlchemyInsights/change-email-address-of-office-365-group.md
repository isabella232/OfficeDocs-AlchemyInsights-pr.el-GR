---
title: Αλλαγή διεύθυνσης ηλεκτρονικού ταχυδρομείου μιας ομάδας Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 32968f085a4e9d49f60ef88e4e78bf6c67629556
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580657"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="706bb-102">Αλλαγή διεύθυνσης ηλεκτρονικού ταχυδρομείου μιας ομάδας Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="706bb-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="706bb-103">Μπορείτε να αλλάξετε τη διεύθυνση ηλεκτρονικού ταχυδρομείου μιας ομάδας Microsoft 365 χρησιμοποιώντας το κέντρο διαχείρισης.</span><span class="sxs-lookup"><span data-stu-id="706bb-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="706bb-104">Απλά επιλέξτε την ομάδα και επιλέξτε @edit διεύθυνση ηλεκτρονικού ταχυδρομείου.</span><span class="sxs-lookup"><span data-stu-id="706bb-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="706bb-105">Μπορείτε επίσης να χρησιμοποιήσετε την ακόλουθη διεύθυνση EXO PowerShell για να αλλάξετε την κύρια διεύθυνση SMTP μιας ομάδας Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="706bb-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

<span data-ttu-id="706bb-106">Ενοποιημένη ομάδα συνόλου <Group Name> -Κύρια διεύθυνση Smtp<new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="706bb-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="706bb-107">Παράδειγμα:</span><span class="sxs-lookup"><span data-stu-id="706bb-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
