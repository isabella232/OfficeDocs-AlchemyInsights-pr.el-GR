---
title: Επιχειρηματικοί κανόνες του Dynamics 365 Forms - Κανόνας επιχείρησης χωρίς ενεργοποίηση για μια φόρμα
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 8425918950e1ef6c44f2866e6fa8987fe165536ae21e08ea6a1da880f761d512
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53947299"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>Το συμβάν OnChange δεν προκύπτει εάν το πεδίο αλλάξει μέσω προγραμματισμού

Το *συμβάν OnChange* δεν προκύπτει εάν το πεδίο αλλάξει μέσω προγραμματισμού χρησιμοποιώντας το *χαρακτηριστικό.* [μέθοδος setValue.](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) Εάν θέλετε τα στοιχεία χειρισμού συμβάντων για το συμβάν *OnChange* να εκτελούνται μετά τον ορισμό της τιμής, πρέπει να χρησιμοποιήσετε τη μέθοδο [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) χαρακτηριστικού *formContext.data.entity* στον κώδικά σας.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
