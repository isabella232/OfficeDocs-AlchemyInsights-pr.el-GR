---
title: Dynamics 365 Forms Business Rules-κανόνας Business not ψήσιμο για μια φόρμα
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
ms.openlocfilehash: 7422b67973f93ce10c1639209cc50206a1016c10
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711491"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a><span data-ttu-id="89e60-102">Το συμβάν OnChange δεν εμφανίζεται εάν το πεδίο έχει αλλάξει μέσω προγραμματισμού</span><span class="sxs-lookup"><span data-stu-id="89e60-102">OnChange event does not occur if the field is changed programmatically</span></span>

<span data-ttu-id="89e60-103">Το συμβάν *OnChange* δεν εμφανίζεται εάν το πεδίο αλλάξει μέσω προγραμματισμού χρησιμοποιώντας το *χαρακτηριστικό.* μέθοδος " [Ορισμός τιμής](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) ".</span><span class="sxs-lookup"><span data-stu-id="89e60-103">The *OnChange* event does not occur if the field is changed programmatically using the *attribute.*[setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) method.</span></span> <span data-ttu-id="89e60-104">Εάν θέλετε τα προγράμματα χειρισμού συμβάντων για το συμβάν *OnChange* να εκτελεστούν μετά τον ορισμό της τιμής, πρέπει να χρησιμοποιήσετε τη μέθοδο [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) *formContext. Data. οντότητας* στον κώδικά σας.</span><span class="sxs-lookup"><span data-stu-id="89e60-104">If you want event handlers for the *OnChange* event to run after you set the value you must use the *formContext.data.entity attribute* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) method in your code.</span></span>

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
