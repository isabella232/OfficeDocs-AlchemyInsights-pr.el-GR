---
title: Επίλυση προβλημάτων ελέγχου ταυτότητας SMTP
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 2d3f0f6b700c3e4485c9064fbaa4bcc165e92e17
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826415"
---
# <a name="solving-smtp-authentication-issues"></a><span data-ttu-id="056e9-102">Επίλυση προβλημάτων ελέγχου ταυτότητας SMTP</span><span class="sxs-lookup"><span data-stu-id="056e9-102">Solving SMTP authentication issues</span></span>

<span data-ttu-id="056e9-103">Εάν εμφανίζεται σφάλμα 5.7.57 ή 5.7.3 κατά την προσπάθεια αποστολής ηλεκτρονικού ταχυδρομείου SMTP και ελέγχου ταυτότητας με ένα πρόγραμμα-πελάτη ή εφαρμογή, υπάρχουν μερικά πράγματα που πρέπει να ελέγξετε:</span><span class="sxs-lookup"><span data-stu-id="056e9-103">If you are getting errors 5.7.57 or 5.7.3 when trying to send SMTP email and authenticate with a client or application, there are a few things you should check:</span></span>

- <span data-ttu-id="056e9-104">Η υποβολή SMTP με έλεγχο ταυτότητας μπορεί να είναι απενεργοποιημένη στο μισθωτή σας ή στο γραμματοκιβώτιο που προσπαθείτε να χρησιμοποιήσετε (ελέγξτε και τις δύο ρυθμίσεις).</span><span class="sxs-lookup"><span data-stu-id="056e9-104">Authenticated SMTP submission might be disabled in your tenant, or on the mailbox that you are trying to use (check both settings).</span></span> <span data-ttu-id="056e9-105">Για να διαβάσετε περισσότερα, ανατρέξτε στο θέμα [Ενεργοποίηση ή απενεργοποίηση υποβολής SMTP προγράμματος-πελάτη με έλεγχο ταυτότητας.](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission)</span><span class="sxs-lookup"><span data-stu-id="056e9-105">To read more, see [Enable or disable authenticated client SMTP submission](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span></span>

- <span data-ttu-id="056e9-106">Ελέγξτε εάν οι [προεπιλογές ασφαλείας Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) είναι ενεργοποιημένες για το μισθωτή σας. Εάν είναι ενεργοποιημένος, ο έλεγχος ταυτότητας SMTP με χρήση βασικού ελέγχου ταυτότητας (γνωστός και ως παλαιού τύπου, θα χρησιμοποιηθεί όνομα χρήστη και κωδικός πρόσβασης) θα αποτύχει.</span><span class="sxs-lookup"><span data-stu-id="056e9-106">Check whether [Azure Security Defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) are enabled for your tenant; if enabled, SMTP authentication using basic authentication (also known as legacy; this will use username and password) will fail.</span></span>
