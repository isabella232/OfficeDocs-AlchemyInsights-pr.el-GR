---
title: Πρόβλημα ενεργοποίησης - Δεν είναι δυνατή η σύνδεση αυτή τη στιγμή
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
- "3408"
- "9001423"
ms.openlocfilehash: 5dad4b43efac2468b57351a4d6c96379ed505071ca144ec0aa518e975633bb18
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998152"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Διόρθωση των Microsoft 365 εφαρμογών "Δεν είναι δυνατή η σύνδεση αυτή τη στιγμή"

Εάν λάβετε αυτό το μήνυμα, δοκιμάστε τα εξής:

1. Ελέγξτε το τείχος προστασίας, το λογισμικό προστασίας από ιούς και τις ρυθμίσεις διακομιστή μεσολάβησης για να επιβεβαιώσετε ότι δεν εμποδίζουν την πρόσβαση στο Internet Microsoft 365 εφαρμογές. Ανατρέξτε [στις διευθύνσεις URL και τις περιοχές διευθύνσεων IP της Microsoft.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Μεταβείτε στην **"Έναρξη**  >  **εκτέλεσης"** και, στη συνέχεια, **πληκτρολογήστε services.msc.** Βεβαιωθείτε ότι εκτελούνται όλες οι ακόλουθες υπηρεσίες:
    - Αυτόματη εγκατάσταση συνδεδεμένων συσκευών δικτύου
    - Υπηρεσία λίστας δικτύου
    - Αναγνώριση τοποθεσίας δικτύου
    - Windows Αρχείο καταγραφής συμβάντων

Εάν κάποια από αυτές τις υπηρεσίες δεν εκτελείται, προσπαθήστε να την ξεκινήσετε. Εάν έχετε κάποιο πρόβλημα κατά την εκκίνηση της υπηρεσίας, εκτελέστε την ακόλουθη εντολή ανοίγοντας μια γραμμή εντολών με αναβαθμισμένα δικαιώματα:

**sfc /scannow**

Αφού ολοκληρωθεί αυτή η εντολή, επανεκκινήστε τον υπολογιστή.

Για λεπτομερείς πληροφορίες, [ανατρέξτε στο θέμα "Λυπούμαστε, δεν είναι δυνατή η σύνδεση με το λογαριασμό σας. Προσπαθήστε ξανά αργότερα" κατά την ενεργοποίηση του Office από Microsoft 365.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)