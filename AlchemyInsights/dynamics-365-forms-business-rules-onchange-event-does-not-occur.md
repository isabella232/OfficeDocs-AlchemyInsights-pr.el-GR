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
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 10/29/2019
ms.locfileid: "37769339"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a><span data-ttu-id="fcd8f-102">Το συμβάν OnChange δεν παρουσιάζεται αν το πεδίο αλλάζει μέσω προγραμματισμού</span><span class="sxs-lookup"><span data-stu-id="fcd8f-102">OnChange event does not occur if the field is changed programmatically</span></span>

<span data-ttu-id="fcd8f-103">Το συμβάν *OnChange* δεν παρουσιάζεται εάν το πεδίο αλλάζει μέσω προγραμματισμού χρησιμοποιώντας το *χαρακτηριστικό.* μέθοδος [SetValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) .</span><span class="sxs-lookup"><span data-stu-id="fcd8f-103">The *OnChange* event does not occur if the field is changed programmatically using the *attribute.*[setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) method.</span></span> <span data-ttu-id="fcd8f-104">Εάν θέλετε τα προγράμματα χειρισμού συμβάντων για το συμβάν *OnChange* να εκτελεστεί αφού ορίσετε την τιμή, πρέπει να χρησιμοποιήσετε τη μέθοδο *formcontext. Data. οντότητα χαρακτηριστικό* [fireonchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) στον κώδικά σας.</span><span class="sxs-lookup"><span data-stu-id="fcd8f-104">If you want event handlers for the *OnChange* event to run after you set the value you must use the *formContext.data.entity attribute* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) method in your code.</span></span>

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
