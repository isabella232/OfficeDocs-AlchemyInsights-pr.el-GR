---
title: AntiSpam 5.4.1 DBEB αλιευμάτων-όλα
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
ms.openlocfilehash: ad0f4c691a5e06306dbb408f4d66a4e00609e4d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43707911"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Επιδιόρθωση ζητημάτων παράδοσης για τον κωδικό σφάλματος 550 5.4.1 Δεν επιτρέπεται η πρόσβαση αναμετάδοσης

Αυτό το ζήτημα παρουσιάζεται κατά [τον έλεγχο για να δείτε εάν μια διεύθυνση ηλεκτρονικού ταχυδρομείου είναι έγκυρη για την αποτροπή bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) κατά την είσοδο στο δίκτυο της Microsoft. Δοκιμάστε τα εξής:

1. Προσδιορίστε αν το πρόβλημα αφορά συγκεκριμένο τομέα ή μία διεύθυνση ηλεκτρονικού ταχυδρομείου:
    - Ολόκληρος τομέας: Μερικές φορές ο τομέας πρέπει να συγχρονιστεί. δοκιμάστε [να ορίζετε τον τομέα σε Εσωτερικό και, στη συνέχεια, να επιστρέψετε στο Έγκυρο](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Ενιαία διεύθυνση ηλεκτρονικού ταχυδρομείου: Μερικές φορές η διεύθυνση πρέπει να συγχρονιστεί. Η αλλαγή της διεύθυνσης διακομιστή μεσολάβησης SMTP και, στη συνέχεια, η αλλαγή της προς τα πίσω μπορεί να βοηθήσει.
2. Προσδιορίστε εάν το ζήτημα αφορά συγκεκριμένα μια ομάδα ή έναν δημόσιο φάκελο. Για ορισμένους τύπους αντικειμένων, τα αντικείμενα ίσως χρειαστεί να δημιουργηθούν με μη αυτόματο τρόπο στην υπηρεσία καταλόγου Azure Active Directory.

Εάν χρειάζεστε πρόσθετη βοήθεια, ανοίξτε ένα δελτίο υποστήριξης και καθορίστε το εύρος του ζητήματος (συμπεριλαμβανομένου του τύπου του αντικειμένου στο οποίο στέλνετε), ώστε να μπορούμε να σας βοηθήσουμε καλύτερα.