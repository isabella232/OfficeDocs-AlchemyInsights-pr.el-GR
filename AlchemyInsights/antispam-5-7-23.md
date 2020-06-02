---
title: Αντιανεπιθύμητη αλληλογραφία - 5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 8122b409a731a5fcc46c718aff1eeda07e26890b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506443"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Επιδιόρθωση ζητημάτων παράδοσης ηλεκτρονικού ταχυδρομείου για τον κωδικό σφάλματος 5.7.23

Επαληθεύστε την εγγραφή SPF DNS για τον τομέα σας σε έναν δημόσια διαθέσιμο έλεγχο εγγραφής SPF ή DNS στο web.

Βεβαιωθείτε ότι το εξερχόμενο μήνυμα δεν προσδιορίστηκε ως ανεπιθύμητο από τη Microsoft και δρομολογήθηκε μέσω του [χώρου συγκέντρωσης παράδοσης υψηλού κινδύνου](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages). Τα μηνύματα στο χώρο συγκέντρωσης παράδοσης υψηλού κινδύνου δεν θα περάσουν τους ελέγχους SPF και, επομένως, δεν θα γίνονται αποδεκτά από τον οργανισμό ηλεκτρονικού ταχυδρομείου προορισμού.

Εάν το πρόβλημα παραμένει, ίσως χρειαστεί να επικοινωνήσετε με το διαχειριστή του κεντρικού υπολογιστή αλληλογραφίας στον οποίο προσπαθείτε να στείλετε μηνύματα ηλεκτρονικού ταχυδρομείου. Σημειώστε το λεπτομερές εξωτερικό σφάλμα που είναι διαθέσιμο στο μήνυμα αναπήδησης. Η υποστήριξη της Microsoft ενδέχεται να μην είναι σε θέση να βοηθήσει περαιτέρω.
