---
title: AggregateGroupMailbox πλήρης έκθεση NDR που ελήφθη για το ηλεκτρονικό ταχυδρομείο που στάλθηκε στο Microsoft 365 Group
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
ms.openlocfilehash: 9de09ab4cbd2f09648305b11da6273ed990907cf
ms.sourcegitcommit: 2ffdf6096de5608b117c6677d3cd7dd4c23ea024
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 12/18/2020
ms.locfileid: "49721920"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>AggregateGroupMailbox πλήρης έκθεση NDR που ελήφθη για το ηλεκτρονικό ταχυδρομείο που στάλθηκε στο Microsoft 365 Group

Χρησιμοποιήστε την ακόλουθη εντολή έξω κέλυφος για να δημιουργήσετε έναν κανόνα μεταφοράς του Exchange για να αποθέσετε μηνύματα ηλεκτρονικού ταχυδρομείου που αποστέλλονται στο συγκεντρωτικό γραμματοκιβώτιο ομάδας:

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

> [!NOTE]
> Αντικαταστήστε τη διεύθυνση SMTP in **-SentTo** με τη διεύθυνση SMTP του γραμματοκιβωτίου ομάδας συγκεντρωτικών αποτελεσμάτων στο μισθωτή σας. Μπορείτε να λάβετε τη διεύθυνση SMTP του γραμματοκιβωτίου ομάδας συγκεντρωτικών αποτελεσμάτων από το NDR Received.



