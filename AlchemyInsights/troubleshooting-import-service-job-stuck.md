---
title: Η αντιμετώπιση προβλημάτων της εργασίας υπηρεσίας εισαγωγής έχει κολλήσει
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/27/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7907"
- "9003046"
ms.openlocfilehash: 987383037f843d347477c0becc859c663736a676
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52125108"
---
# <a name="troubleshooting-import-service-job-stuck"></a><span data-ttu-id="2ac8d-102">Η αντιμετώπιση προβλημάτων της εργασίας υπηρεσίας εισαγωγής έχει κολλήσει</span><span class="sxs-lookup"><span data-stu-id="2ac8d-102">Troubleshooting Import Service job stuck</span></span>

<span data-ttu-id="2ac8d-103">Εάν αντιμετωπίζετε προβλήματα με την εισαγωγή εργασιών υπηρεσίας που έχουν κολλήσει ή αποτύχει, εξετάστε και δοκιμάστε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="2ac8d-103">If you are experiencing issues with Import service jobs stuck or failing, examine and try the following:</span></span>

- <span data-ttu-id="2ac8d-104">Εξετάστε το μέγεθος του αρχείου PST.</span><span class="sxs-lookup"><span data-stu-id="2ac8d-104">Review the size of of the PST file.</span></span> <span data-ttu-id="2ac8d-105">Το μέγιστο προτεινόμενο μέγεθος ενός αρχείου PST για εισαγωγή είναι 20 GB.</span><span class="sxs-lookup"><span data-stu-id="2ac8d-105">The maximum recommended size of a PST file for import is 20GB.</span></span>

- <span data-ttu-id="2ac8d-106">Εάν υποπτεύεστε ότι τα στοιχεία που έχουν παραλειφθεί λόγω καταστροφής, εκτελέστε Scanpst.exe να διαγνώσετε και να διορθώσετε σφάλματα σε αρχεία PST.</span><span class="sxs-lookup"><span data-stu-id="2ac8d-106">If you suspect skipped items due to corruption, run Scanpst.exe to diagnose and fix errors in PST files.</span></span>

- <span data-ttu-id="2ac8d-107">Εάν εμφανιστεί ένα σφάλμα "MapiExceptionShutoffQuotaExceeded" κατά την εισαγωγή, βεβαιωθείτε ότι το γραμματοκιβώτιο προορισμού έχει επαρκή χωρητικότητα για την εισαγωγή των αρχείων PST που θέλετε.</span><span class="sxs-lookup"><span data-stu-id="2ac8d-107">If you see a "MapiExceptionShutoffQuotaExceeded" error during import, make sure the target mailbox has sufficient capacity to import the desired PST files.</span></span>

<span data-ttu-id="2ac8d-108">Για περισσότερες πληροφορίες σχετικά με την αντιμετώπιση προβλημάτων εργασίας εισαγωγής PST, ανατρέξτε στο θέμα [Αντιμετώπιση προβλημάτων με τις εργασίες εισαγωγής PST.](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)</span><span class="sxs-lookup"><span data-stu-id="2ac8d-108">For more information on troubleshooting PST import job issues, see [Troubleshoot issues with PST import jobs](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span></span>

<span data-ttu-id="2ac8d-109">Για πληροφορίες σχετικά με τον τρόπο επιδιόρθωσης προβλημάτων κατά την εισαγωγή PTS στο Outlook, ανατρέξτε στο θέμα Επιδιόρθωση προβλημάτων κατά την εισαγωγή [ενός αρχείου .pst Outlook (microsoft.com).](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us)</span><span class="sxs-lookup"><span data-stu-id="2ac8d-109">For information about how to fix issues when importing PSTs into Outlook, see [Fix problems importing an Outlook .pst file (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us).</span></span>