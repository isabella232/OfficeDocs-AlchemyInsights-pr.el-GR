---
title: Επιδιόρθωση εφαρμογών του Office Λυπούμαστε, έχουμε προσωρινό μήνυμα ζητημάτων διακομιστή
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: a1ac62f3587e318d563cfea1df8db23b720358a6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764117"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a>Επιδιόρθωση του μηνύματος "Λυπούμαστε, έχουμε προσωρινά προβλήματα διακομιστή"

Εάν λάβετε αυτό το μήνυμα, δοκιμάστε τα εξής:

1. Ελέγξτε το τείχος προστασίας, το λογισμικό προστασίας από ιούς και τις ρυθμίσεις διακομιστή μεσολάβησης, για να επιβεβαιώσετε ότι δεν εμποδίζουν την πρόσβαση στο Internet στις εφαρμογές του Office. Ανατρέξτε [στην περιοχή URL και διευθύνσεων IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Μεταβείτε **στην έναρξη** > **εκτέλεσης**και, στη συνέχεια, πληκτρολογήστε **services.msc**. Βεβαιωθείτε ότι εκτελούνται όλες οι ακόλουθες υπηρεσίες:
    - Αυτόματη εγκατάσταση συνδεδεμένων συσκευών δικτύου
    - Υπηρεσία λίστας δικτύου
    - Ευαισθητοποίηση τοποθεσίας δικτύου
    - Αρχείο καταγραφής συμβάντων των Windows

Εάν μία από αυτές τις υπηρεσίες δεν εκτελείται, προσπαθήστε να την ξεκινήσετε. Εάν αντιμετωπίσετε πρόβλημα κατά την εκκίνηση της υπηρεσίας, εκτελέστε την ακόλουθη εντολή ανοίγοντας μια γραμμή εντολών με αυξημένα δικαιώματα:

**sfc /scannow**

Μετά την ολοκλήρωση αυτής της εντολής, κάντε επανεκκίνηση του υπολογιστή.

Για λεπτομερείς πληροφορίες, [ανατρέξτε στην ενότητα "Λυπούμαστε, δεν μπορούμε να συνδεθούμε στο λογαριασμό σας. Προσπαθήστε ξανά αργότερα" σφάλμα κατά την ενεργοποίηση](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)του .