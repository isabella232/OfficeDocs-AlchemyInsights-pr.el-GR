---
title: Αντιspam 5.4.1 DBEB αλιευμάτων-όλα
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: 4f531a063d63aff239ef7dead869bb526e17fb35
ms.sourcegitcommit: 2591e1f56e8943bddb9d3b77ba5b494ac49d4f30
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 11/15/2019
ms.locfileid: "38672433"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Επιδιόρθωση ζητημάτων παράδοσης για τον κωδικό σφάλματος 550 5.4.1 δεν επιτρέπεται η πρόσβαση αναμετάδοσης

Αυτό το ζήτημα παρουσιάζεται κατά [τον έλεγχο για να δείτε εάν μια διεύθυνση ηλεκτρονικού ταχυδρομείου είναι έγκυρη για να αποτρέψετε τις επικράσεις](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) κατά την είσοδο στο δίκτυο του Office 365. Δοκιμάστε τα εξής:

1. Προσδιορίστε αν το πρόβλημα αφορά έναν ολόκληρο τομέα ή μια μεμονωμένη διεύθυνση ηλεκτρονικού ταχυδρομείου:
    - Ολόκληρος τομέας: μερικές φορές ο τομέας πρέπει να συγχρονιστεί. Προσπαθήστε [να ρυθμίσετε τον τομέα σε εσωτερικό και, στη συνέχεια, πίσω στην επίσημη](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Μεμονωμένη διεύθυνση ηλεκτρονικού ταχυδρομείου: μερικές φορές η διεύθυνση πρέπει να συγχρονιστεί. αλλαγή της διεύθυνσης διακομιστή μεσολάβησης SMTP και, στη συνέχεια, η αλλαγή του πίσω μπορεί να βοηθήσει.
2. Προσδιορίστε αν το πρόβλημα αφορά συγκεκριμένη ομάδα ή δημόσιο φάκελο. Για ορισμένους τύπους αντικειμένων, τα αντικείμενα ενδέχεται να χρειαστεί να δημιουργηθούν με μη αυτόματο τρόπο στο Azure Active Directory.

Αν χρειάζεστε επιπλέον βοήθεια, ανοίξτε ένα εισιτήριο υποστήριξης και καθορίστε το πεδίο εφαρμογής του θέματος (συμπεριλαμβανομένου του τύπου του αντικειμένου που στέλνετε), ώστε να μπορούμε να σας βοηθήσουμε καλύτερα.