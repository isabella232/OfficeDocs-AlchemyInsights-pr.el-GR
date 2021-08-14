---
title: Η πλήρης NDR του AggregateGroupMailbox λήφθηκε για μηνύματα ηλεκτρονικού ταχυδρομείου που στάλθηκαν Microsoft 365 ομάδα
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004286"
- "7656"
ms.openlocfilehash: 6655bbe9482400eeb3cfdf0b91bdc595e3d98fbff0f6d9244db8bb4dd958305e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951853"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>Η πλήρης NDR του AggregateGroupMailbox λήφθηκε για μηνύματα ηλεκτρονικού ταχυδρομείου που στάλθηκαν Microsoft 365 ομάδα

Χρησιμοποιήστε την ακόλουθη εντολή "Κέλυφος EXO" για να δημιουργήσετε έναν Exchange μεταφοράς για σιωπηρή απόθεση μηνυμάτων ηλεκτρονικού ταχυδρομείου που αποστέλλονται στο γραμματοκιβώτιο ομάδας συγκεντρωτικών αποτελεσμάτων:

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

> [!NOTE]
> Αντικαταστήστε τη διεύθυνση SMTP στο **-SentTo με** τη διεύθυνση SMTP του γραμματοκιβωτίου συγκεντρωτικών ομάδων στο μισθωτή σας. Μπορείτε να λάβετε τη διεύθυνση SMTP του γραμματοκιβωτίου ομάδας συγκεντρωτικών αποτελεσμάτων από την NDR που λάβατε.



