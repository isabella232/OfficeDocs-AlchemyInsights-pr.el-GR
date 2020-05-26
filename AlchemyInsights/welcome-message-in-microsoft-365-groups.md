---
title: Μήνυμα υποδοχής στις ομάδες του Microsoft 365
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
- "5685"
ms.openlocfilehash: d82931ae6978a09e674b00640d1dd413bcce7cfd
ms.sourcegitcommit: b196100759b29aecd62b693a2bfedbbd25a697c6
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44357536"
---
# <a name="welcome-message-in-microsoft-365-groups"></a>Μήνυμα υποδοχής στις ομάδες του Microsoft 365

Οι νέοι χρήστες που συμμετέχουν στην ομάδα Microsoft 365 θα λάβουν μηνύματα ηλεκτρονικού ταχυδρομείου υποδοχής εάν η ιδιότητα "UnifiedGroupWelcomeMessageEnabled" είναι αληθής.

Σε περίπτωση που θέλετε να απενεργοποιήσετε το μήνυμα υποδοχής, χρησιμοποιήστε την ακόλουθη εντολή [EXO PowerShell:](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps)

`
Set-UnifiedGroup <groupname> -UnifiedGroupWelcomeMessageEnabled:$False
`
