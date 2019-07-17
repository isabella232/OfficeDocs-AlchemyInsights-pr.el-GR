---
title: Dynamics 365 αποτελεί επιχειρησιακών κανόνων - επιχειρησιακός κανόνας δεν γίνεται πυροδότηση για μια φόρμα
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 4ade8d2f68b465298e2d6efff3eef4f04f25c3bf
ms.sourcegitcommit: a413a0e27ef4ab8c484fa9fccff8bbef381c8b96
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35747713"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>Συμβάν OnChange δεν παρουσιάζεται, αν το πεδίο έχει αλλάξει μέσω προγραμματισμού

Το συμβάν *OnChange* δεν παρουσιάζεται αν το πεδίο έχει αλλάξει μέσω προγραμματισμού, χρησιμοποιώντας το *χαρακτηριστικό.* η μέθοδος ["Ορισμός τιμής"](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) . Εάν θέλετε τα προγράμματα χειρισμού συμβάντων για το συμβάν *OnChange* για να εκτελείται αφού ορίσετε την τιμή που πρέπει να χρησιμοποιήσετε το *το χαρακτηριστικό formContext.data.entity.* η μέθοδος [fireOnchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) στον κώδικά σας.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
