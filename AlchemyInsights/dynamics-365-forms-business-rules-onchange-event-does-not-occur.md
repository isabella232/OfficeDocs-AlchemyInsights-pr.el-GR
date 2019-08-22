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
ms.openlocfilehash: cbdedd2c5fcf5517243e60e36d86479d6c3f7814
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529019"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>Συμβάν OnChange δεν παρουσιάζεται, αν το πεδίο έχει αλλάξει μέσω προγραμματισμού

Το συμβάν *OnChange* δεν παρουσιάζεται αν το πεδίο έχει αλλάξει μέσω προγραμματισμού, χρησιμοποιώντας το *χαρακτηριστικό.* η μέθοδος ["Ορισμός τιμής"](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) . Εάν θέλετε τα προγράμματα χειρισμού συμβάντων για το συμβάν *OnChange* για να εκτελείται αφού ορίσετε την τιμή που πρέπει να χρησιμοποιήσετε το *το χαρακτηριστικό formContext.data.entity.* η μέθοδος [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) στον κώδικά σας.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
