---
title: Επιδιόρθωση εφαρμογών του Microsoft 365 Δυστυχώς, έχουμε ένα μήνυμα προσωρινών προβλημάτων διακομιστή
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
- "3420"
- "9001430"
ms.openlocfilehash: 0adf1d66869051b9dd8290ef3466ef9b13aa2d41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835271"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Επιδιόρθωση των εφαρμογών του Microsoft 365 "Λυπούμαστε, έχουμε προσωρινά προβλήματα διακομιστή"

Εάν λάβετε αυτό το μήνυμα, δοκιμάστε τα εξής:

1. Ελέγξτε το τείχος προστασίας, το λογισμικό προστασίας από ιούς και τις ρυθμίσεις διακομιστή μεσολάβησης για να επιβεβαιώσετε ότι δεν εμποδίζουν την πρόσβαση στο Internet σε εφαρμογές του Microsoft 365. Δείτε [διευθύνσεις URL και περιοχές διευθύνσεων IP.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Μεταβείτε στην **"Έναρξη**  >  **εκτέλεσης"** και, στη συνέχεια, **πληκτρολογήστε services.msc.** Βεβαιωθείτε ότι εκτελούνται όλες οι ακόλουθες υπηρεσίες:
    - Αυτόματη εγκατάσταση συνδεδεμένων συσκευών δικτύου
    - Υπηρεσία λίστας δικτύου
    - Αναγνώριση τοποθεσίας δικτύου
    - Αρχείο καταγραφής συμβάντων των Windows

Εάν κάποια από αυτές τις υπηρεσίες δεν εκτελείται, προσπαθήστε να την ξεκινήσετε. Εάν έχετε κάποιο πρόβλημα κατά την εκκίνηση της υπηρεσίας, εκτελέστε την ακόλουθη εντολή ανοίγοντας μια γραμμή εντολών με αναβαθμισμένα δικαιώματα:

**sfc /scannow**

Αφού ολοκληρωθεί αυτή η εντολή, επανεκκινήστε τον υπολογιστή.

Για λεπτομερείς πληροφορίες, [ανατρέξτε στο θέμα "Λυπούμαστε, δεν είναι δυνατή η σύνδεση με το λογαριασμό σας. Προσπαθήστε ξανά αργότερα" κατά την ενεργοποίηση.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)