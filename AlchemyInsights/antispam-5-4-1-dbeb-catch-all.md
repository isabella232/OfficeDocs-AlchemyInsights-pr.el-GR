---
title: AntiSpam 5.4.1 DBEB catch-all
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
- "9001209"
- "3167"
ms.openlocfilehash: c6ce26a133428dc7351912d8250ef096dfc7521a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821447"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Επιδιόρθωση προβλημάτων παράδοσης για τον κωδικό σφάλματος 550 5.4.1 Δεν επιτρέπεται η πρόσβαση αναμετάδοσης

Αυτό το πρόβλημα παρουσιάζεται [όταν ελέγχετε εάν μια διεύθυνση ηλεκτρονικού ταχυδρομείου είναι](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) έγκυρη για την αποτροπή επιστροφών κατά την είσοδο στο δίκτυο της Microsoft. Δοκιμάστε τα εξής:

1. Προσδιορίστε εάν το πρόβλημα αφορά έναν ολόκληρο τομέα ή μία διεύθυνση ηλεκτρονικού ταχυδρομείου:
    - Ολόκληρος ο τομέας: Μερικές φορές ο τομέας πρέπει να συγχρονιστεί. δοκιμάστε [να ορίσετε τον τομέα σε "Εσωτερικό" και, στη συνέχεια, να τον ορίσετε ξανά ως "Επίσημο".](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)
    - Μία διεύθυνση ηλεκτρονικού ταχυδρομείου: Ορισμένες φορές η διεύθυνση πρέπει να συγχρονιστεί. Η αλλαγή της διεύθυνσης διακομιστή μεσολάβησης smtp και, στη συνέχεια, η επιστροφή της μπορεί να σας βοηθήσει.
2. Προσδιορίστε εάν το πρόβλημα αφορά συγκεκριμένα μια ομάδα ή έναν δημόσιο φάκελο. Για ορισμένους τύπους αντικειμένων, τα αντικείμενα ενδέχεται να πρέπει να δημιουργηθούν με μη αυτόματο τρόπο στο Azure Active Directory.

Εάν χρειάζεστε επιπλέον βοήθεια, ανοίξτε ένα δελτίο υποστήριξης και καθορίστε το εύρος του προβλήματος (συμπεριλαμβανομένου του τύπου του αντικειμένου στο οποίο στέλνετε) ώστε να σας βοηθήσουμε καλύτερα.