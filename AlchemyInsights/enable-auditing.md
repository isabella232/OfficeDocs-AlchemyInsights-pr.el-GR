---
title: Ενεργοποίηση και αναζητήστε το αρχείο καταγραφής ελέγχου
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "286"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 8c965cb1c2b6a4cb46b5c1b0145932c4c54ba97d
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270528"
---
# <a name="enable-and-search-audit-log"></a><span data-ttu-id="760c2-102">Ενεργοποίηση και αναζητήστε το αρχείο καταγραφής ελέγχου</span><span class="sxs-lookup"><span data-stu-id="760c2-102">Enable and search Audit log</span></span>

<span data-ttu-id="760c2-103">Για να αναζητήσετε το αρχείο καταγραφής ελέγχου του Office 365, ακολουθήστε [τα εξής βήματα](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="760c2-103">To search the Office 365 audit log, follow [these steps](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>

<span data-ttu-id="760c2-104">**Ανταλλαγή**</span><span class="sxs-lookup"><span data-stu-id="760c2-104">**Exchange**</span></span>

- <span data-ttu-id="760c2-105">Δραστηριότητες διαχείρισης Exchange ελέγχονται από προεπιλογή.</span><span class="sxs-lookup"><span data-stu-id="760c2-105">Exchange admin activities are audited by default.</span></span>

- <span data-ttu-id="760c2-106">Είμαστε στη διαδικασία Ενεργοποίηση ελέγχου γραμματοκιβωτίου από προεπιλογή στο Office 365.</span><span class="sxs-lookup"><span data-stu-id="760c2-106">We are in the process of enabling mailbox auditing by default in Office 365.</span></span> <span data-ttu-id="760c2-107">Μέχρι τότε, για να ενεργοποιήσετε τον έλεγχο για ένα μόνο γραμματοκιβώτιο ή για όλα τα γραμματοκιβώτια στον οργανισμό σας, ανατρέξτε στην ενότητα [αυτού του άρθρου](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing).</span><span class="sxs-lookup"><span data-stu-id="760c2-107">Until then, to enable auditing for a single mailbox or for all mailboxes in your organization, see  [this article](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing).</span></span>

- <span data-ttu-id="760c2-108">Office 365 ομάδα γραμματοκιβώτια και δημόσιου φακέλου γραμματοκιβώτια στο Exchange Online δεν υποστηρίζει αρχεία καταγραφής ελέγχου.</span><span class="sxs-lookup"><span data-stu-id="760c2-108">Office 365 Group mailboxes and public folder mailboxes in Exchange Online don't support audit logging.</span></span>

<span data-ttu-id="760c2-109">**Του SharePoint και OneDrive**</span><span class="sxs-lookup"><span data-stu-id="760c2-109">**SharePoint and OneDrive**</span></span>

- <span data-ttu-id="760c2-110">Δεν υπάρχει καμία πρόσθετη ρύθμιση παραμέτρων που απαιτείται για να ενεργοποιήσετε τον έλεγχο του SharePoint και OneDrive.</span><span class="sxs-lookup"><span data-stu-id="760c2-110">There's no additional configuration required to enable auditing for SharePoint and OneDrive.</span></span>

- <span data-ttu-id="760c2-111">Του SharePoint και OneDrive υποστηρίζουν τον έλεγχο τους ακόλουθους τύπους δραστηριοτήτων:</span><span class="sxs-lookup"><span data-stu-id="760c2-111">SharePoint and OneDrive support auditing the following types of activities:</span></span>

    - <span data-ttu-id="760c2-112">Αρχείο, φάκελο και δραστηριότητες σελίδα</span><span class="sxs-lookup"><span data-stu-id="760c2-112">File, folder, and page activities</span></span>
    - <span data-ttu-id="760c2-113">Κοινή χρήση και πρόσβαση σε δραστηριότητες</span><span class="sxs-lookup"><span data-stu-id="760c2-113">Sharing and access request activities</span></span>
    - <span data-ttu-id="760c2-114">Δραστηριότητες διαχείρισης τοποθεσίας</span><span class="sxs-lookup"><span data-stu-id="760c2-114">Site administration activities</span></span>
    - <span data-ttu-id="760c2-115">Αρχείο δραστηριοτήτων συγχρονισμού</span><span class="sxs-lookup"><span data-stu-id="760c2-115">File synchronization activities</span></span>

- <span data-ttu-id="760c2-116">Για πληροφορίες σχετικά με δραστηριότητες ελέγχονται σε άλλες υπηρεσίες του Office 365, ανατρέξτε [στον πίνακα σε αυτό το άρθρο](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#audited-activities).</span><span class="sxs-lookup"><span data-stu-id="760c2-116">For information about audited activities in other Office 365 services, see  [the table in this article](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#audited-activities).</span></span>

- <span data-ttu-id="760c2-117">Εδώ μια λίστα με συνήθεις ερωτήσεις [συχνές ερωτήσεις](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#frequently-asked-questions) σχετικά με την αναζήτηση στο αρχείο καταγραφής ελέγχου.</span><span class="sxs-lookup"><span data-stu-id="760c2-117">Here a list of frequently asked questions [frequently asked questions](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#frequently-asked-questions) about searching the audit log.</span></span>