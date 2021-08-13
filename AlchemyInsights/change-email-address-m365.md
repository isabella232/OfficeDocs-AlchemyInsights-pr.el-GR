---
title: Αλλαγή διεύθυνσης ηλεκτρονικού ταχυδρομείου μιας ομάδας του Microsoft 365 ή του Microsoft Teams
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
ms.openlocfilehash: acb343553bfb7e100c03d0e7046ed5cbdd6b739b9a61e3faf17768bd8aadff34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53995622"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Αλλαγή διεύθυνσης ηλεκτρονικού ταχυδρομείου μιας ομάδας του Microsoft 365 ή του Microsoft Teams

Μπορείτε να αλλάξετε τη διεύθυνση ηλεκτρονικού ταχυδρομείου μιας ομάδας του Microsoft 365 ή του Microsoft Teams, χρησιμοποιώντας το [Κέντρο διαχείρισης Microsoft 365](https://admin.microsoft.com/). Απλώς επιλέξτε την ομάδα και, στη συνέχεια, επιλέξτε @επεξεργασία διεύθυνσης ηλεκτρονικού ταχυδρομείου.

Μπορείτε επίσης να χρησιμοποιήσετε την ακόλουθη εντολή EXO PowerShell για να αλλάξετε την κύρια διεύθυνση SMTP μιας ομάδας του Microsoft 365 ή του Teams:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Παράδειγμα:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
