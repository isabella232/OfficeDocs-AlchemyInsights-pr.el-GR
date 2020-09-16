---
title: Επιδιόρθωση εφαρμογών του Microsoft 365 Λυπούμαστε, αντιμετωπίζουμε προσωρινά μηνύματα προβλημάτων διακομιστή
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
- "3420"
- "9001430"
ms.openlocfilehash: e00504d318efdea4968ddf98b3ce9591f8993e38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758245"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Επιδιόρθωση των εφαρμογών του Microsoft 365 "Λυπούμαστε, αντιμετωπίζουμε προβλήματα προσωρινού διακομιστή"

Εάν λάβετε αυτό το μήνυμα, δοκιμάστε τα εξής:

1. Επιλέξτε το τείχος προστασίας, το λογισμικό προστασίας από ιούς και τις ρυθμίσεις του διακομιστή μεσολάβησης για να επιβεβαιώσετε ότι δεν εμποδίζουν την πρόσβαση στο Internet στις εφαρμογές Microsoft 365. Ανατρέξτε στο θέμα [διευθύνσεις URL και περιοχές διευθύνσεων IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Μεταβείτε στην **Έναρξη**  >  **εκτέλεση**και, στη συνέχεια, πληκτρολογήστε **Services. msc**. Βεβαιωθείτε ότι όλες οι υπηρεσίες που ακολουθούν εκτελούνται:
    - Αυτόματη ρύθμιση συσκευών με σύνδεση δικτύου
    - Υπηρεσία λίστας δικτύου
    - Συνειδητοποίηση τοποθεσίας δικτύου
    - Αρχείο καταγραφής συμβάντων των Windows

Εάν μία από αυτές τις υπηρεσίες δεν εκτελείται, προσπαθήστε να την εκκινήσετε. Εάν αντιμετωπίζετε πρόβλημα κατά την εκκίνηση της υπηρεσίας, εκτελέστε την ακόλουθη εντολή, ανοίγοντας μια γραμμή εντολών με αναβαθμισμένα δικαιώματα:

**sfc/scannow**

Μετά την ολοκλήρωση αυτής της εντολής, επανεκκινήστε τον υπολογιστή.

Για λεπτομερείς πληροφορίες, ανατρέξτε [στο θέμα "Λυπούμαστε, δεν είναι δυνατή η σύνδεση με το λογαριασμό σας. Παρακαλούμε δοκιμάστε ξανά αργότερα "σφάλμα κατά την ενεργοποίηση](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).