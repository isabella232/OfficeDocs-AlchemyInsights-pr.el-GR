---
title: Αλλαγή διεύθυνσης ηλεκτρονικού ταχυδρομείου μιας Microsoft 365 ομάδας
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 6bd9301b983d09f6a0058fee17577b9fc695458ed205f96aacf79a87e4a91e34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930729"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Αλλαγή διεύθυνσης ηλεκτρονικού ταχυδρομείου μιας Microsoft 365 ομάδας

Μπορείτε να αλλάξετε τη διεύθυνση ηλεκτρονικού ταχυδρομείου μιας Microsoft 365 ομάδας χρησιμοποιώντας το κέντρο διαχείρισης. Απλώς επιλέξτε την ομάδα και, στη συνέχεια, επιλέξτε @επεξεργασία διεύθυνσης ηλεκτρονικού ταχυδρομείου.

Μπορείτε επίσης να χρησιμοποιήσετε την εντολή EXO PowerShell για να αλλάξετε την κύρια διεύθυνση SMTP μιας Microsoft 365 ομάδας:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>

Παράδειγμα:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
