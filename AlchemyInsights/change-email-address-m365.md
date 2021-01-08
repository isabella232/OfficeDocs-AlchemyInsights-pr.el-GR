---
title: Αλλαγή διεύθυνσης ηλεκτρονικού ταχυδρομείου μιας ομάδας του Microsoft 365 ή του Microsoft Teams
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
ms.openlocfilehash: ff7abaf3d8e0ed977eba5712bdd19185738fa75c
ms.sourcegitcommit: 8be59778b7d39213a27a471802eae7fc006eb1ff
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 01/05/2021
ms.locfileid: "49756557"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Αλλαγή διεύθυνσης ηλεκτρονικού ταχυδρομείου μιας ομάδας του Microsoft 365 ή του Microsoft Teams

Μπορείτε να αλλάξετε τη διεύθυνση ηλεκτρονικού ταχυδρομείου μιας ομάδας του Microsoft 365 ή του Microsoft Teams, χρησιμοποιώντας το [Κέντρο διαχείρισης Microsoft 365](https://admin.microsoft.com/). Απλώς επιλέξτε την ομάδα και, στη συνέχεια, επιλέξτε @επεξεργασία διεύθυνσης ηλεκτρονικού ταχυδρομείου.

Μπορείτε επίσης να χρησιμοποιήσετε την ακόλουθη εντολή EXO PowerShell για να αλλάξετε την κύρια διεύθυνση SMTP μιας ομάδας του Microsoft 365 ή του Teams:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Παράδειγμα:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
