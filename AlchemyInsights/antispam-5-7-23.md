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
ms.openlocfilehash: cb9073306c65b09813290d6c8470d14395d2836fa3048f8ce0ecb8b06e71a010
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932169"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Επιδιόρθωση προβλημάτων παράδοσης ηλεκτρονικού ταχυδρομείου για τον κωδικό σφάλματος 5.7.23

Επαληθεύστε την εγγραφή DNS SPF για τον τομέα σας σε έναν δημόσια διαθέσιμο έλεγχο SPF ή εγγραφής DNS στο web.

Βεβαιωθείτε ότι το εξερχόμενο μήνυμα δεν έχει αναγνωριστεί ως ανεπιθύμητη αλληλογραφία από τη Microsoft και δρομολογήθηκε μέσω του [χώρου συγκέντρωσης παράδοσης υψηλού κινδύνου.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages) Τα μηνύματα στο χώρο συγκέντρωσης παράδοσης υψηλού κινδύνου δεν θα περάσουν από ελέγχους SPF και, επομένως, δεν θα γίνουν αποδεκτά από τον οργανισμό ηλεκτρονικού ταχυδρομείου προορισμού.

Εάν το πρόβλημα παραμένει, ίσως χρειαστεί να επικοινωνήσετε με το διαχειριστή του κεντρικού υπολογιστή αλληλογραφίας στον οποίο προσπαθείτε να στείλετε μηνύματα ηλεκτρονικού ταχυδρομείου. Σημειώστε το λεπτομερές εξωτερικό σφάλμα που είναι διαθέσιμο στο μήνυμα αναπήδησης. Η υποστήριξη της Microsoft ενδέχεται να μην μπορεί να βοηθήσει περαιτέρω.
