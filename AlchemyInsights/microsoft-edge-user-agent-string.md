---
title: Συμβολοσειρά παράγοντα χρήστη του Microsoft Edge (επιφάνεια εργασίας)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003862"
- "6914"
ms.openlocfilehash: b4106dde1e09e0ce07b4b9adc2b2984cc5609c3b
ms.sourcegitcommit: 3c6e777d6679a24108171e9aa3f9379a8d44e001
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 12/09/2020
ms.locfileid: "49678100"
---
# <a name="microsoft-edge-user-agent-string-desktop"></a><span data-ttu-id="e72a2-102">Συμβολοσειρά παράγοντα χρήστη του Microsoft Edge (επιφάνεια εργασίας)</span><span class="sxs-lookup"><span data-stu-id="e72a2-102">Microsoft Edge user agent string (Desktop)</span></span>

<span data-ttu-id="e72a2-103">Οι συμβολοσειρές παράγοντα χρήστη (UA) μπορούν να χρησιμοποιηθούν για τον εντοπισμό της έκδοσης ενός συγκεκριμένου προγράμματος περιήγησης που χρησιμοποιείται σε ένα συγκεκριμένο λειτουργικό σύστημα.</span><span class="sxs-lookup"><span data-stu-id="e72a2-103">User agent (UA) strings can be used to detect what version of a specific browser is being used on a certain operating system.</span></span> <span data-ttu-id="e72a2-104">Όπως και σε άλλα προγράμματα περιήγησης, το Microsoft Edge περιλαμβάνει αυτές τις πληροφορίες στην κεφαλίδα HTTP "User-Agent" κάθε φορά που κάνει μια αίτηση σε μια τοποθεσία.</span><span class="sxs-lookup"><span data-stu-id="e72a2-104">Like other browsers, Microsoft Edge includes this information in the "User-Agent" HTTP header whenever it makes a request to a site.</span></span> <span data-ttu-id="e72a2-105">Μπορείτε επίσης να αποκτήσετε πρόσβαση στις πληροφορίες έκδοσης του προγράμματος περιήγησης μέσω JavaScript, πραγματοποιώντας ερώτημα σχετικά με την τιμή "Navigator. παράγοντα".</span><span class="sxs-lookup"><span data-stu-id="e72a2-105">The browser-version information can also be accessed via JavaScript by querying the value of "navigator.userAgent".</span></span>

<span data-ttu-id="e72a2-106">Συνιστούμε στους προγραμματιστές Web να χρησιμοποιούν τον εντοπισμό δυνατοτήτων κάθε φορά που είναι εφικτό, για να βελτιώσουν τη διατήρηση του κώδικα, να μειώσουν την αστάθεια του κώδικα και να εξαλείψουν τον κίνδυνο θραύσης του κώδικα σε περίπτωση μελλοντικών ενημερώσεων σειράς UA.</span><span class="sxs-lookup"><span data-stu-id="e72a2-106">We recommend that web developers make use of feature detection whenever possible to improve code maintainability, reduce code fragility, and eliminate the risk of code breakage in the event of future UA string updates.</span></span>

<span data-ttu-id="e72a2-107">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [συμβολοσειρά παράγοντα χρήστη του Microsoft Edge (επιφάνεια εργασίας)](https://docs.microsoft.com/microsoft-edge/web-platform/user-agent-string).</span><span class="sxs-lookup"><span data-stu-id="e72a2-107">For more information, see [Microsoft Edge User Agent String (Desktop)](https://docs.microsoft.com/microsoft-edge/web-platform/user-agent-string).</span></span>