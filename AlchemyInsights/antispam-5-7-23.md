---
title: Ανεπιθύμητη αλληλογραφία-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: ecbce4f0077dc9acab63575c19d40c0675a406ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717325"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Επιδιόρθωση ζητημάτων παράδοσης ηλεκτρονικού ταχυδρομείου για τον κωδικό σφάλματος 5.7.23

Επαληθεύστε την εγγραφή DNS SPF για τον τομέα σας σε έναν δημόσια διαθέσιμο έλεγχο εγγραφής SPF ή DNS στο Web.

Βεβαιωθείτε ότι το εξερχόμενο μήνυμα δεν αναγνωρίστηκε ως ανεπιθύμητη αλληλογραφία από τη Microsoft και ότι δρομολογείται μέσω του [χώρου συγκέντρωσης παράδοσης υψηλού κινδύνου](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages). Τα μηνύματα στο χώρο συγκέντρωσης παράδοσης υψηλού κινδύνου δεν μεταβιβάζουν τους ελέγχους SPF και, επομένως, δεν θα γίνονται δεκτά από τον οργανισμό ηλεκτρονικού ταχυδρομείου προορισμού.

Εάν το πρόβλημα δεν επιλυθεί, ίσως χρειαστεί να επικοινωνήσετε με το διαχειριστή του κεντρικού υπολογιστή αλληλογραφίας στον οποίο επιχειρείτε να στείλετε μήνυμα ηλεκτρονικού ταχυδρομείου. Σημειώστε το λεπτομερές εξωτερικό σφάλμα που είναι διαθέσιμο στο μήνυμα αναπήδησης. Η υποστήριξη της Microsoft ενδέχεται να μην είναι σε θέση να σας βοηθήσει περαιτέρω.
