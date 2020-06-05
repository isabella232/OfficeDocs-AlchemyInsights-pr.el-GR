---
title: Ζήτημα ενεργοποίησης - Δεν είναι δυνατή η σύνδεση αυτήν τη στιγμή
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: b46bac60633ad9a006b9446919b8c99e221b07e4
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44581875"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Επιδιόρθωση του μηνύματος "Δεν είναι δυνατή η σύνδεση των εφαρμογών microsoft 365 αυτήν τη στιγμή"

Εάν λάβετε αυτό το μήνυμα, δοκιμάστε τα εξής:

1. Ελέγξτε το τείχος προστασίας, το λογισμικό προστασίας από ιούς και τις ρυθμίσεις διακομιστή μεσολάβησης, για να επιβεβαιώσετε ότι δεν εμποδίζουν την πρόσβαση στο Internet σε εφαρμογές της Microsoft 365. Ανατρέξτε στο θέμα [Διευθύνσεις URL της Microsoft και περιοχές διευθύνσεων IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Μεταβείτε **στην έναρξη**  >  **εκτέλεσης**και, στη συνέχεια, πληκτρολογήστε **services.msc**. Βεβαιωθείτε ότι εκτελούνται όλες οι ακόλουθες υπηρεσίες:
    - Αυτόματη εγκατάσταση συνδεδεμένων συσκευών δικτύου
    - Υπηρεσία λίστας δικτύου
    - Ευαισθητοποίηση τοποθεσίας δικτύου
    - Αρχείο καταγραφής συμβάντων των Windows

Εάν μία από αυτές τις υπηρεσίες δεν εκτελείται, προσπαθήστε να την ξεκινήσετε. Εάν αντιμετωπίσετε πρόβλημα κατά την εκκίνηση της υπηρεσίας, εκτελέστε την ακόλουθη εντολή ανοίγοντας μια γραμμή εντολών με αυξημένα δικαιώματα:

**sfc /scannow**

Μετά την ολοκλήρωση αυτής της εντολής, κάντε επανεκκίνηση του υπολογιστή.

Για λεπτομερείς πληροφορίες, [ανατρέξτε στην ενότητα "Λυπούμαστε, δεν μπορούμε να συνδεθούμε στο λογαριασμό σας. Προσπαθήστε ξανά αργότερα" σφάλμα κατά την ενεργοποίηση του Office από το Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).