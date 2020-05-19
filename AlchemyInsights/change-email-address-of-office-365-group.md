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
# <a name="change-email-address-of-an-microsoft-365-group"></a>Αλλαγή διεύθυνσης ηλεκτρονικού ταχυδρομείου μιας ομάδας microsoft 365

Μπορείτε να αλλάξετε τη διεύθυνση ηλεκτρονικού ταχυδρομείου μιας ομάδας Microsoft 365 χρησιμοποιώντας το κέντρο διαχείρισης. Απλά επιλέξτε την ομάδα και επιλέξτε @edit διεύθυνση ηλεκτρονικού ταχυδρομείου.

Μπορείτε επίσης να χρησιμοποιήσετε την ακόλουθη διεύθυνση EXO PowerShell για να αλλάξετε την κύρια διεύθυνση SMTP μιας ομάδας Microsoft 365:

Ενοποιημένη ομάδα συνόλου <Group Name> -Κύρια διεύθυνση Smtp<new SMTP Address>

Παράδειγμα:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
