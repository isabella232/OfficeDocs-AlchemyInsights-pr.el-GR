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
# <a name="solving-smtp-authentication-issues"></a>Επίλυση προβλημάτων ελέγχου ταυτότητας SMTP

Εάν εμφανίζεται σφάλμα 5.7.57 ή 5.7.3 κατά την προσπάθεια αποστολής ηλεκτρονικού ταχυδρομείου SMTP και ελέγχου ταυτότητας με ένα πρόγραμμα-πελάτη ή εφαρμογή, υπάρχουν μερικά πράγματα που πρέπει να ελέγξετε:

- Η υποβολή SMTP με έλεγχο ταυτότητας μπορεί να είναι απενεργοποιημένη στο μισθωτή σας ή στο γραμματοκιβώτιο που προσπαθείτε να χρησιμοποιήσετε (ελέγξτε και τις δύο ρυθμίσεις). Για να διαβάσετε περισσότερα, ανατρέξτε στο θέμα [Ενεργοποίηση ή απενεργοποίηση υποβολής SMTP προγράμματος-πελάτη με έλεγχο ταυτότητας.](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission)

- Ελέγξτε εάν οι [προεπιλογές ασφαλείας Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) είναι ενεργοποιημένες για το μισθωτή σας. Εάν είναι ενεργοποιημένος, ο έλεγχος ταυτότητας SMTP με χρήση βασικού ελέγχου ταυτότητας (γνωστός και ως παλαιού τύπου, θα χρησιμοποιηθεί όνομα χρήστη και κωδικός πρόσβασης) θα αποτύχει.
