---
title: Αλλαγή διεύθυνσης ηλεκτρονικού ταχυδρομείου μιας ομάδας microsoft 365
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
ms.openlocfilehash: 0a07e6279f533a4c26a4e90c10651421a5df8860
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/27/2020
ms.locfileid: "44282924"
---
# <a name="change-email-address-of-an-microsoft-365-group"></a><span data-ttu-id="0426b-102">Αλλαγή διεύθυνσης ηλεκτρονικού ταχυδρομείου μιας ομάδας microsoft 365</span><span class="sxs-lookup"><span data-stu-id="0426b-102">Change email address of an Microsoft 365 group</span></span>

<span data-ttu-id="0426b-103">Μπορείτε να αλλάξετε τη διεύθυνση ηλεκτρονικού ταχυδρομείου μιας ομάδας Microsoft 365 χρησιμοποιώντας το κέντρο διαχείρισης.</span><span class="sxs-lookup"><span data-stu-id="0426b-103">You can change the email address of an Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="0426b-104">Απλά επιλέξτε την ομάδα και επιλέξτε @edit διεύθυνση ηλεκτρονικού ταχυδρομείου.</span><span class="sxs-lookup"><span data-stu-id="0426b-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="0426b-105">Μπορείτε επίσης να χρησιμοποιήσετε την ακόλουθη διεύθυνση EXO PowerShell για να αλλάξετε την κύρια διεύθυνση SMTP μιας ομάδας Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="0426b-105">You can also use following the EXO PowerShell command to change the primary SMTP address of an Microsoft 365 group:</span></span>

<span data-ttu-id="0426b-106">Ενοποιημένη ομάδα συνόλου <Group Name> -Κύρια διεύθυνση Smtp<new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="0426b-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="0426b-107">Παράδειγμα:</span><span class="sxs-lookup"><span data-stu-id="0426b-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
