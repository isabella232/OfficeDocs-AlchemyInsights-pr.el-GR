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
ms.openlocfilehash: 4b90f843843416408d7f3091325fe436dc3ec9df
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627990"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a>Επιδιόρθωση των εφαρμογών του Office "Λυπούμαστε, έχουμε προσωρινά ζητήματα διακομιστή" μήνυμα

Εάν λάβετε αυτό το μήνυμα, δοκιμάστε τα εξής:

1. Ελέγξτε το τείχος προστασίας, το λογισμικό προστασίας από ιούς και τις ρυθμίσεις διακομιστή μεσολάβησης για να επιβεβαιώσετε ότι δεν εμποδίζουν την πρόσβαση στο Internet σε εφαρμογές του Office. Δείτε [διευθύνσεις URL του Office 365 και περιοχές διευθύνσεων IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Μεταβείτε στην **Έναρξη** > **εκτέλεσης**και, στη συνέχεια, πληκτρολογήστε **Services. msc**. Βεβαιωθείτε ότι εκτελούνται όλες οι ακόλουθες υπηρεσίες:
    - Αυτόματη εγκατάσταση συνδεδεμένων συσκευών δικτύου
    - Υπηρεσία λίστας δικτύου
    - Ενημέρωση τοποθεσίας δικτύου
    - Αρχείο καταγραφής συμβάντων των Windows

Εάν μια από αυτές τις υπηρεσίες δεν εκτελείται, προσπαθήστε να την ξεκινήσετε. Εάν έχετε πρόβλημα με την εκκίνηση της υπηρεσίας, εκτελέστε την ακόλουθη εντολή ανοίγοντας μια γραμμή εντολών με αυξημένα δικαιώματα:

**sfc/scannow**

Μετά την ολοκλήρωση αυτής της εντολής, επανεκκινήστε τον υπολογιστή.

Για αναλυτικές πληροφορίες, ανατρέξτε [στην «Λυπούμαστε, δεν μπορούμε να συνδεθούμε με το λογαριασμό σας. Προσπαθήστε ξανά αργότερα "σφάλμα κατά την ενεργοποίηση του Office από 365 του Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).