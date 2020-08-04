---
title: Χρήση καταγραφής χρήσης για τη Διαχείριση δικαιωμάτων Azure
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5506"
- "9002281"
ms.openlocfilehash: 606fcdc5394edab26c60925af28cf2d938aac172
ms.sourcegitcommit: 1dada930649a2625eb6d15910b2bfd5e1e00e5b6
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/03/2020
ms.locfileid: "46555126"
---
# <a name="use-usage-logging-for-azure-rights-management"></a><span data-ttu-id="8b407-102">Χρήση καταγραφής χρήσης για τη Διαχείριση δικαιωμάτων Azure</span><span class="sxs-lookup"><span data-stu-id="8b407-102">Use usage logging for Azure Rights Management</span></span>

<span data-ttu-id="8b407-103">Από προεπιλογή, η καταγραφή χρήσης προστασίας είναι ενεργοποιημένη για όλους τους πελάτες.</span><span class="sxs-lookup"><span data-stu-id="8b407-103">By default, protection usage logging is enabled for all customers.</span></span> <span data-ttu-id="8b407-104">Τα αρχεία καταγραφής εγγράφονται ως μια σειρά αντικειμένων blob στο χώρο αποθήκευσης Azure για τον μισθωτή σας.</span><span class="sxs-lookup"><span data-stu-id="8b407-104">Logs are written as a series of blobs in Azure storage for your tenant.</span></span> <span data-ttu-id="8b407-105">Μετά από μια ενέργεια προστασίας, ενδέχεται να χρειαστούν έως και 15 λεπτά για να εμφανιστούν τα περισσότερα αρχεία καταγραφής.</span><span class="sxs-lookup"><span data-stu-id="8b407-105">After a protection action, it might take up to 15 minutes for most logs to appear.</span></span>

<span data-ttu-id="8b407-106">Μπορείτε να χρησιμοποιήσετε αρχεία καταγραφής χρήσης προστασίας για να κάνετε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="8b407-106">You can use protection usage logs to:</span></span>

- <span data-ttu-id="8b407-107">Ανάλυση επιχειρηματικών πληροφοριών</span><span class="sxs-lookup"><span data-stu-id="8b407-107">Analyze business insights</span></span>

- <span data-ttu-id="8b407-108">Παρακολούθηση για κατάχρηση</span><span class="sxs-lookup"><span data-stu-id="8b407-108">Monitor for abuse</span></span>

- <span data-ttu-id="8b407-109">Εκτέλεση εγκληματολογικής ανάλυσης</span><span class="sxs-lookup"><span data-stu-id="8b407-109">Perform forensic analysis</span></span>

<span data-ttu-id="8b407-110">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Καταγραφή και ανάλυση της χρήσης προστασίας από την Προστασία πληροφοριών Azure](https://docs.microsoft.com/azure/information-protection/log-analyze-usage).</span><span class="sxs-lookup"><span data-stu-id="8b407-110">For more information, see [Logging and analyzing the protection usage from Azure Information Protection](https://docs.microsoft.com/azure/information-protection/log-analyze-usage).</span></span>

<span data-ttu-id="8b407-111">Για πληροφορίες σχετικά με την καταγραφή χρήσης υπολογιστή-πελάτη, ανατρέξτε στον [Οδηγό διαχείρισης: Αρχεία προγράμματος-πελάτη Προστασίας πληροφοριών Azure και καταγραφή χρήσης προγράμματος-πελάτη](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-files-and-logging).</span><span class="sxs-lookup"><span data-stu-id="8b407-111">For information about client usage logging, see [Admin Guide: Azure Information Protection client files and client usage logging](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-files-and-logging).</span></span>

<span data-ttu-id="8b407-112">Για περισσότερες πληροφορίες, ανατρέξτε στα θέματα:</span><span class="sxs-lookup"><span data-stu-id="8b407-112">For additional information, see:</span></span>

- <span data-ttu-id="8b407-113">[Απαιτήσεις προστασίας πληροφοριών Azure](https://docs.microsoft.com/azure/information-protection/get-started/requirements).</span><span class="sxs-lookup"><span data-stu-id="8b407-113">[Azure Information Protection requirements](https://docs.microsoft.com/azure/information-protection/get-started/requirements).</span></span>
    
- <span data-ttu-id="8b407-114">[Πρόγραμμα εκμάθησης: Ρυθμίστε τις παραμέτρους πολιτικής προστασίας πληροφοριών Azure και δημιουργήστε μια νέα ετικέτα](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial).</span><span class="sxs-lookup"><span data-stu-id="8b407-114">[Tutorial: Configure Azure Information Protection policy settings and create a new label](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial).</span></span>