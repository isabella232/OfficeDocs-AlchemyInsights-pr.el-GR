---
title: Antispam-5.7.23
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
ms.openlocfilehash: 9c9bc2d04fb8efaa5e75194b4ca09316d24e018e
ms.sourcegitcommit: 07b47d7f3ca191363e6bc84140e8e01524d6f08e
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 10/24/2019
ms.locfileid: "37682146"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Επιδιόρθωση ζητημάτων παράδοσης ηλεκτρονικού ταχυδρομείου για τον κωδικό σφάλματος 5.7.23

Επαληθεύστε την εγγραφή SPF DNS για τον τομέα σας σε ένα δημόσια διαθέσιμο SPF ή ελεγκτή εγγραφών DNS στο Web.

Βεβαιωθείτε ότι το εξερχόμενο μήνυμα δεν αναγνωρίστηκε ως ανεπιθύμητο από το Office 365 και δρομολογείται μέσω του [χώρου συγκέντρωσης υψηλών κινδύνων](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages). Τα μηνύματα στο χώρο συγκέντρωσης υψηλού κινδύνου δεν περνούν τους ελέγχους SPF και επομένως δεν θα γίνουν αποδεκτά από τον οργανισμό ηλεκτρονικού ταχυδρομείου προορισμού.

Εάν το πρόβλημα επιμείνει, ίσως χρειαστεί να επικοινωνήσετε με το διαχειριστή του κεντρικού υπολογιστή αλληλογραφίας στον οποίο επιχειρείτε να στείλετε μηνύματα ηλεκτρονικού ταχυδρομείου. Σημειώστε το λεπτομερές εξωτερικό σφάλμα που είναι διαθέσιμο στο μήνυμα ανάκλασης.  Η υποστήριξη του Office 365 ενδέχεται να μην μπορεί να βοηθήσει περαιτέρω.