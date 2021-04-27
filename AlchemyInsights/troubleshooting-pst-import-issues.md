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
ms.openlocfilehash: 5065b9895954371e4298c98e8aadb67ba8f140fd
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52059815"
---
# <a name="troubleshooting-pst-import-issues"></a><span data-ttu-id="5a844-102">Αντιμετώπιση προβλημάτων με την εισαγωγή αρχείων PST</span><span class="sxs-lookup"><span data-stu-id="5a844-102">Troubleshooting PST import issues</span></span>

- <span data-ttu-id="5a844-103">Εάν κάνετε εισαγωγή μέσα στο ίδιο το πρόγραμμα-πελάτη του Outlook, ανατρέξτε στο θέμα [Επιδιόρθωση προβλημάτων εισαγωγής ενός αρχείου .pst του Outlook.](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e)</span><span class="sxs-lookup"><span data-stu-id="5a844-103">If you are importing within the Outlook client itself, see [Fix problems importing an Outlook .pst file](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span></span>

- <span data-ttu-id="5a844-104">Εάν χρησιμοποιείτε την Υπηρεσία εισαγωγής και έχει κολλήσει, σημειώστε ότι κάθε αρχείο PST που αποστέλλετε στη θέση αποθήκευσης Azure δεν πρέπει να είναι μεγαλύτερο από 20 GB.</span><span class="sxs-lookup"><span data-stu-id="5a844-104">If you are using Import Service and it's stuck, note that each PST file that you upload to the Azure Storage location should be no larger than 20GB.</span></span> <span data-ttu-id="5a844-105">Τα αρχεία PST που είναι μεγαλύτερα από 20 GB ενδέχεται να επηρεάσουν τις επιδόσεις της διαδικασίας εισαγωγής PST.</span><span class="sxs-lookup"><span data-stu-id="5a844-105">PST files larger than 20GB may impact the performance of the PST import process.</span></span> <span data-ttu-id="5a844-106">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα Θέματα που επηρεάζουν [τις εργασίες εισαγωγής PST.](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)</span><span class="sxs-lookup"><span data-stu-id="5a844-106">For more information troubleshooting stuck jobs, see [Issues that affect PST import jobs](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span></span>

- <span data-ttu-id="5a844-107">Εάν θέλετε να επαληθεύσετε την κατάσταση μιας συγκεκριμένης εργασίας εισαγωγής, χρησιμοποιήστε τη [λειτουργία Get-MailboxImportRequest -batchname.](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest)</span><span class="sxs-lookup"><span data-stu-id="5a844-107">If you want to verify the status of a specific Import job, use [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span></span>

- <span data-ttu-id="5a844-108">Για πλήρεις λεπτομέρειες σχετικά με την υπηρεσία εισαγωγής, [ανατρέξτε στο θέμα Επισκόπηση της εισαγωγής των αρχείων PST του οργανισμού σας.](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="5a844-108">For full details on the import service, see [Overview of importing your organization's PST files](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span></span>
