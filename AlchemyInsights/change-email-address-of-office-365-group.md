---
title: Αλλαγή διεύθυνσης ηλεκτρονικού ταχυδρομείου μιας ομάδας Microsoft 365
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
ms.openlocfilehash: 8eaafae8650a8072cdfbec281afe6d5e93fea655
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819044"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Αλλαγή διεύθυνσης ηλεκτρονικού ταχυδρομείου μιας ομάδας Microsoft 365

Μπορείτε να αλλάξετε τη διεύθυνση ηλεκτρονικού ταχυδρομείου μιας ομάδας Microsoft 365 χρησιμοποιώντας το κέντρο διαχείρισης. Απλώς επιλέξτε την ομάδα και, στη συνέχεια, επιλέξτε @επεξεργασία διεύθυνσης ηλεκτρονικού ταχυδρομείου.

Μπορείτε επίσης να χρησιμοποιήσετε την εντολή EXO PowerShell για να αλλάξετε την κύρια διεύθυνση SMTP μιας ομάδας Microsoft 365:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>

Παράδειγμα:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
