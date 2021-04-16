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
ms.openlocfilehash: 2dd3c97bb85254215b13ee8a1222941c0492b204
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51806442"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Διόρθωση του μηνύματος "Δεν είναι δυνατή η σύνδεση αυτή τη στιγμή" των εφαρμογών Του Microsoft 365

Εάν λάβετε αυτό το μήνυμα, δοκιμάστε τα εξής:

1. Ελέγξτε το τείχος προστασίας, το λογισμικό προστασίας από ιούς και τις ρυθμίσεις διακομιστή μεσολάβησης για να επιβεβαιώσετε ότι δεν εμποδίζουν την πρόσβαση στο Internet σε εφαρμογές του Microsoft 365. Ανατρέξτε [στις διευθύνσεις URL και τις περιοχές διευθύνσεων IP της Microsoft.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Μεταβείτε στην **"Έναρξη**  >  **εκτέλεσης"** και, στη συνέχεια, **πληκτρολογήστε services.msc.** Βεβαιωθείτε ότι εκτελούνται όλες οι ακόλουθες υπηρεσίες:
    - Αυτόματη εγκατάσταση συνδεδεμένων συσκευών δικτύου
    - Υπηρεσία λίστας δικτύου
    - Αναγνώριση τοποθεσίας δικτύου
    - Αρχείο καταγραφής συμβάντων των Windows

Εάν κάποια από αυτές τις υπηρεσίες δεν εκτελείται, προσπαθήστε να την ξεκινήσετε. Εάν έχετε κάποιο πρόβλημα κατά την εκκίνηση της υπηρεσίας, εκτελέστε την ακόλουθη εντολή ανοίγοντας μια γραμμή εντολών με αναβαθμισμένα δικαιώματα:

**sfc /scannow**

Αφού ολοκληρωθεί αυτή η εντολή, επανεκκινήστε τον υπολογιστή.

Για λεπτομερείς πληροφορίες, [ανατρέξτε στο θέμα "Λυπούμαστε, δεν είναι δυνατή η σύνδεση με το λογαριασμό σας. Προσπαθήστε ξανά αργότερα" κατά την ενεργοποίηση του Office από το Microsoft 365.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)