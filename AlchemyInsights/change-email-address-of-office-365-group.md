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
# <a name="change-email-address-of-a-microsoft-365-group"></a>Αλλαγή διεύθυνσης ηλεκτρονικού ταχυδρομείου μιας ομάδας Microsoft 365

Μπορείτε να αλλάξετε τη διεύθυνση ηλεκτρονικού ταχυδρομείου μιας ομάδας Microsoft 365 χρησιμοποιώντας το κέντρο διαχείρισης. Απλά επιλέξτε την ομάδα και επιλέξτε @edit διεύθυνση ηλεκτρονικού ταχυδρομείου.

Μπορείτε επίσης να χρησιμοποιήσετε την ακόλουθη διεύθυνση EXO PowerShell για να αλλάξετε την κύρια διεύθυνση SMTP μιας ομάδας Microsoft 365:

Ενοποιημένη ομάδα συνόλου <Group Name> -Κύρια διεύθυνση Smtp<new SMTP Address>

Παράδειγμα:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
