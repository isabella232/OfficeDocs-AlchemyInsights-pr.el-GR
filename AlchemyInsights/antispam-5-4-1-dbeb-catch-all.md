---
title: Ανεπιθύμητη αλληλογραφία 5.4.1 DBEB catch-all
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
- "9001209"
- "3167"
ms.openlocfilehash: f9d613457ae33dc7e00f20391bbdff029500a123
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717361"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Επιδιόρθωση ζητημάτων παράδοσης για τον κωδικό σφάλματος 550 δεν επιτρέπεται η πρόσβαση 5.4.1 Relay

Αυτό το πρόβλημα παρουσιάζεται κατά [τον έλεγχο για να δείτε εάν μια διεύθυνση ηλεκτρονικού ταχυδρομείου είναι έγκυρη για να αποτρέψετε την επιστροφές](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) κατά την είσοδό σας στο δίκτυο της Microsoft. Δοκιμάστε τα εξής:

1. Προσδιορίστε εάν το πρόβλημα αφορά έναν ολόκληρο τομέα ή μια μεμονωμένη διεύθυνση ηλεκτρονικού ταχυδρομείου:
    - Ολόκληρος ο τομέας: ορισμένες φορές ο τομέας πρέπει να συγχρονιστεί. Δοκιμάστε να [ορίσετε τον τομέα σε εσωτερικό και, στη συνέχεια, επιστρέψτε σε επιτακτικό](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Μεμονωμένη διεύθυνση ηλεκτρονικού ταχυδρομείου: ορισμένες φορές η διεύθυνση πρέπει να συγχρονιστεί. η αλλαγή της διεύθυνσης διακομιστή μεσολάβησης SMTP και, στη συνέχεια, η αλλαγή της πίσω μπορεί να βοηθήσει.
2. Προσδιορίστε εάν το πρόβλημα αφορά συγκεκριμένα μια ομάδα ή έναν δημόσιο φάκελο. Για ορισμένους τύπους αντικειμένων, τα αντικείμενα μπορεί να πρέπει να δημιουργηθούν με μη αυτόματο τρόπο στο Azure Active Directory.

Εάν χρειάζεστε επιπλέον βοήθεια, ανοίξτε ένα δελτίο υποστήριξης και καθορίστε την εμβέλεια του ζητήματος (συμπεριλαμβανομένου του τύπου του αντικειμένου που στέλνετε), ώστε να μπορέσουμε να σας βοηθήσουμε καλύτερα.