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
ms.openlocfilehash: 3cdd2175083e864b3bffc57a70bb6c6220843fad
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 11/15/2019
ms.locfileid: "37769339"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>Το συμβάν OnChange δεν παρουσιάζεται αν το πεδίο αλλάζει μέσω προγραμματισμού

Το συμβάν *OnChange* δεν παρουσιάζεται εάν το πεδίο αλλάζει μέσω προγραμματισμού χρησιμοποιώντας το *χαρακτηριστικό.* μέθοδος [SetValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) . Εάν θέλετε τα προγράμματα χειρισμού συμβάντων για το συμβάν *OnChange* να εκτελεστεί αφού ορίσετε την τιμή, πρέπει να χρησιμοποιήσετε τη μέθοδο *formcontext. Data. οντότητα χαρακτηριστικό* [fireonchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) στον κώδικά σας.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
