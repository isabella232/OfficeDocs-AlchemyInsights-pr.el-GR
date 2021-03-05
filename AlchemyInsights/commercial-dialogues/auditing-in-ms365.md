---
title: Έλεγχος στο Microsoft 365
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: c07981bfae40d74deb1a2f143ce51da69b51a69f
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50482367"
---
# <a name="auditing-in-microsoft-365"></a><span data-ttu-id="f45d3-102">Έλεγχος στο Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="f45d3-102">Auditing in Microsoft 365</span></span>

<span data-ttu-id="f45d3-103">Ακολουθούν ορισμένα πράγματα που πρέπει να γνωρίζετε σχετικά με τον έλεγχο στο Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="f45d3-103">Here are a few things you should know about auditing in Microsoft 365:</span></span>

1. <span data-ttu-id="f45d3-104">Οι δραστηριότητες διαχειριστή του Exchange ελέγχονται από προεπιλογή.</span><span class="sxs-lookup"><span data-stu-id="f45d3-104">Exchange admin activities are audited by default.</span></span>
1. <span data-ttu-id="f45d3-105">Είμαστε στη διαδικασία της ενεργοποίηση του ελέγχου γραμματοκιβωτίου από προεπιλογή για όλους τους χρήστες.</span><span class="sxs-lookup"><span data-stu-id="f45d3-105">We're in the process of turning on mailbox auditing by default for all users.</span></span> <span data-ttu-id="f45d3-106">Για να διαβάσετε περισσότερα σχετικά με αυτό, κάντε κλικ [εδώ.](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Exchange-Mailbox-Auditing-will-be-enabled-by-default/ba-p/215171)</span><span class="sxs-lookup"><span data-stu-id="f45d3-106">To read more about this, click [here](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Exchange-Mailbox-Auditing-will-be-enabled-by-default/ba-p/215171).</span></span> <span data-ttu-id="f45d3-107">Μέχρι τότε, εάν θέλετε οδηγίες για τη μη αυτόματη ενεργοποίηση της δυνατότητας για ένα άτομο ή για έναν ολόκληρο οργανισμό, επιλέξτε το κουμπί "Ενεργοποίηση ελέγχου γραμματοκιβωτίου" παρακάτω.</span><span class="sxs-lookup"><span data-stu-id="f45d3-107">Until then, if you want instructions to manually enable it for one person or an entire organization, choose the Turn on mailbox auditing button below.</span></span>
1. <span data-ttu-id="f45d3-108">Τα γραμματοκιβώτια των Ομάδων Microsoft 365 και τα γραμματοκιβώτια δημόσιων φακέλων δεν υποστηρίζουν την καταγραφή ελέγχου.</span><span class="sxs-lookup"><span data-stu-id="f45d3-108">Microsoft 365 Groups mailboxes and Public Folder mailboxes do not support audit logging.</span></span>
1. <span data-ttu-id="f45d3-109">Για το SharePoint/OneDrive, δεν απαιτείται πρόσθετη ρύθμιση παραμέτρων για την ενεργοποίηση του ελέγχου.</span><span class="sxs-lookup"><span data-stu-id="f45d3-109">For SharePoint/OneDrive, there is no additional configuration required to enabled auditing.</span></span> <span data-ttu-id="f45d3-110">Για να μάθετε ποιες δραστηριότητες ελέγχονται, ανατρέξτε στο θέμα:</span><span class="sxs-lookup"><span data-stu-id="f45d3-110">To learn what activities are audited, see:</span></span>
    1. [<span data-ttu-id="f45d3-111">Δραστηριότητες αρχείων</span><span class="sxs-lookup"><span data-stu-id="f45d3-111">File activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#file-and-page-activities)
    1. [<span data-ttu-id="f45d3-112">Δραστηριότητες φακέλου</span><span class="sxs-lookup"><span data-stu-id="f45d3-112">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    1. <span data-ttu-id="f45d3-113">[Δραστηριότητες κοινής χρήσης και πρόσβασης.](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)</span><span class="sxs-lookup"><span data-stu-id="f45d3-113">[Sharing and Access activities](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities).</span></span>
1. <span data-ttu-id="f45d3-114">Για μια λίστα με όλες τις ελεγχόμενες δραστηριότητες κατά υπηρεσία, ανατρέξτε στο θέμα ["Ελεγχόμενες δραστηριότητες".](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#audited-activities)</span><span class="sxs-lookup"><span data-stu-id="f45d3-114">For a list of all audited activities by service, see [Audited activities](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#audited-activities).</span></span>
