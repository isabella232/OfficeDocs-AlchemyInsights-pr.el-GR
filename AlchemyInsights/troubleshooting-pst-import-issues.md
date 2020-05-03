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
# <a name="troubleshooting-pst-import-issues"></a><span data-ttu-id="2d5aa-102">Αντιμετώπιση προβλημάτων με την εισαγωγή αρχείων PST</span><span class="sxs-lookup"><span data-stu-id="2d5aa-102">Troubleshooting PST import issues</span></span>

- <span data-ttu-id="2d5aa-103">Εάν πραγματοποιείτε εισαγωγή εντός του ίδιου του προγράμματος-πελάτη Outlook, Ανατρέξτε στο θέμα [Επιδιόρθωση προβλημάτων κατά την εισαγωγή ενός αρχείου .pst του Outlook](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span><span class="sxs-lookup"><span data-stu-id="2d5aa-103">If you are importing within the Outlook client itself, please see [Fix problems importing an Outlook .pst file](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span></span>

- <span data-ttu-id="2d5aa-104">Εάν χρησιμοποιείτε την υπηρεσία εισαγωγής και έχει κολλήσει, έχετε υπόψη ότι κάθε αρχείο PST που αποστέλλετε στη θέση της υπηρεσίας αποθήκευσης Microsoft Azure δεν πρέπει να υπερβαίνει τα 20 GB.</span><span class="sxs-lookup"><span data-stu-id="2d5aa-104">If you are using Import Service and it is stuck, please note that each PST file that you upload to the Azure Storage location should be no larger than 20 GB.</span></span> <span data-ttu-id="2d5aa-105">Τα αρχεία PST που είναι μεγαλύτερα από 20 GB ενδέχεται να επηρεάσουν την απόδοση της διαδικασίας εισαγωγής PST.</span><span class="sxs-lookup"><span data-stu-id="2d5aa-105">PST files larger than 20 GB may impact the performance of the PST import process.</span></span>

- <span data-ttu-id="2d5aa-106">Εάν θέλετε να επαληθεύσετε την κατάσταση μιας συγκεκριμένης εργασίας εισαγωγής, μπορείτε να χρησιμοποιήσετε το [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span><span class="sxs-lookup"><span data-stu-id="2d5aa-106">If you want to verify the status of a specific Import job, you can use [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span></span>

- <span data-ttu-id="2d5aa-107">Για λεπτομερείς πληροφορίες σχετικά με την υπηρεσία εισαγωγής, ανατρέξτε στο θέμα [Επισκόπηση της εισαγωγής αρχείων PST του οργανισμού σας](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="2d5aa-107">For full details on the import service, please see [Overview of importing your organization's PST files](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span></span>
