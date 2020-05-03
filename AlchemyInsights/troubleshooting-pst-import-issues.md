---
title: Αντιμετώπιση προβλημάτων με την εισαγωγή αρχείων PST
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1225"
ms.openlocfilehash: 58fdd509fae5e87bf5ae72db5d8926c4367cdd64
ms.sourcegitcommit: 87aa36e3ff4835efb120a320c5169bfa77199ec4
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 05/01/2020
ms.locfileid: "43991237"
---
# <a name="troubleshooting-pst-import-issues"></a>Αντιμετώπιση προβλημάτων με την εισαγωγή αρχείων PST

- Εάν πραγματοποιείτε εισαγωγή εντός του ίδιου του προγράμματος-πελάτη Outlook, Ανατρέξτε στο θέμα [Επιδιόρθωση προβλημάτων κατά την εισαγωγή ενός αρχείου .pst του Outlook](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).

- Εάν χρησιμοποιείτε την υπηρεσία εισαγωγής και έχει κολλήσει, έχετε υπόψη ότι κάθε αρχείο PST που αποστέλλετε στη θέση της υπηρεσίας αποθήκευσης Microsoft Azure δεν πρέπει να υπερβαίνει τα 20 GB. Τα αρχεία PST που είναι μεγαλύτερα από 20 GB ενδέχεται να επηρεάσουν την απόδοση της διαδικασίας εισαγωγής PST.

- Εάν θέλετε να επαληθεύσετε την κατάσταση μιας συγκεκριμένης εργασίας εισαγωγής, μπορείτε να χρησιμοποιήσετε το [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).

- Για λεπτομερείς πληροφορίες σχετικά με την υπηρεσία εισαγωγής, ανατρέξτε στο θέμα [Επισκόπηση της εισαγωγής αρχείων PST του οργανισμού σας](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).
