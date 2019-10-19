---
title: Dynamics 365 φόρμες επιχειρηματικές κανόνες-κανόνας επιχείρησης δεν πυροδότηση για μια φόρμα
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: cbdedd2c5fcf5517243e60e36d86479d6c3f7814
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 10/18/2019
ms.locfileid: "36529019"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>Το συμβάν OnChange δεν παρουσιάζεται αν το πεδίο αλλάζει μέσω προγραμματισμού

Το συμβάν *OnChange* δεν παρουσιάζεται εάν το πεδίο αλλάζει μέσω προγραμματισμού χρησιμοποιώντας το *χαρακτηριστικό.* μέθοδος [SetValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) . Εάν θέλετε τα προγράμματα χειρισμού συμβάντων για το συμβάν *OnChange* να εκτελεστεί αφού ορίσετε την τιμή, πρέπει να χρησιμοποιήσετε το *χαρακτηριστικό formcontext. Data. οντότητας.* μέθοδος [Fireonchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) στον κώδικά σας.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
