---
title: Αντιμετώπιση προβλημάτων με την εισαγωγή αρχείων PST
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1225"
ms.openlocfilehash: 549af832f9c58db1cdd8fbe80b8b5bd2aba9bd937f33116806a9391cbc9a5d4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972419"
---
# <a name="troubleshooting-pst-import-issues"></a>Αντιμετώπιση προβλημάτων με την εισαγωγή αρχείων PST

- Εάν κάνετε εισαγωγή μέσα στο ίδιο το Outlook, ανατρέξτε στο θέμα Επιδιόρθωση προβλημάτων κατά [την εισαγωγή Outlook αρχείου .pst.](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e)

- Εάν χρησιμοποιείτε την υπηρεσία εισαγωγής και έχει κολλήσει, σημειώστε ότι κάθε αρχείο PST που αποστέλλετε στη θέση του Azure Υπηρεσία αποθήκευσης δεν πρέπει να είναι μεγαλύτερο από 20 GB. Τα αρχεία PST που είναι μεγαλύτερα από 20 GB ενδέχεται να επηρεάσουν τις επιδόσεις της διαδικασίας εισαγωγής PST. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα Θέματα που επηρεάζουν [τις εργασίες εισαγωγής PST.](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)

- Εάν θέλετε να επαληθεύσετε την κατάσταση μιας συγκεκριμένης εργασίας εισαγωγής, χρησιμοποιήστε τη [λειτουργία Get-MailboxImportRequest -batchname.](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest)

- Για πλήρεις λεπτομέρειες σχετικά με την υπηρεσία εισαγωγής, [ανατρέξτε στο θέμα Επισκόπηση της εισαγωγής των αρχείων PST του οργανισμού σας.](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide)
