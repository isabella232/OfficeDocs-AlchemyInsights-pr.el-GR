---
title: Antispam - 5.7.23
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: e494e8017f24d65a94d1a7490be4d67c46a2120b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821411"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Επιδιόρθωση προβλημάτων παράδοσης ηλεκτρονικού ταχυδρομείου για τον κωδικό σφάλματος 5.7.23

Επαληθεύστε την εγγραφή DNS SPF για τον τομέα σας σε έναν δημόσια διαθέσιμο έλεγχο SPF ή εγγραφής DNS στο web.

Βεβαιωθείτε ότι το εξερχόμενο μήνυμα δεν έχει αναγνωριστεί ως ανεπιθύμητη αλληλογραφία από τη Microsoft και δρομολογήθηκε μέσω του [χώρου συγκέντρωσης παράδοσης υψηλού κινδύνου.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages) Τα μηνύματα στο χώρο συγκέντρωσης παράδοσης υψηλού κινδύνου δεν θα περάσουν από ελέγχους SPF και, επομένως, δεν θα γίνουν αποδεκτά από τον οργανισμό ηλεκτρονικού ταχυδρομείου προορισμού.

Εάν το πρόβλημα παραμένει, ίσως χρειαστεί να επικοινωνήσετε με το διαχειριστή του κεντρικού υπολογιστή αλληλογραφίας στον οποίο προσπαθείτε να στείλετε μηνύματα ηλεκτρονικού ταχυδρομείου. Σημειώστε το λεπτομερές εξωτερικό σφάλμα που είναι διαθέσιμο στο μήνυμα αναπήδησης. Η υποστήριξη της Microsoft ενδέχεται να μην μπορεί να βοηθήσει περαιτέρω.
