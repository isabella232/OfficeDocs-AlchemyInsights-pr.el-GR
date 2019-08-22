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
ms.openlocfilehash: 37ffbe6a3c94edc3b9888b1544e9e29097d3425a
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36527723"
---
# <a name="enable-and-search-the-audit-log"></a><span data-ttu-id="3cea9-102">Ενεργοποίηση και αναζητήστε το αρχείο καταγραφής ελέγχου</span><span class="sxs-lookup"><span data-stu-id="3cea9-102">Enable and search the Audit log</span></span>

<span data-ttu-id="3cea9-103">Για να αναζητήσετε το αρχείο καταγραφής ελέγχου του Office 365, ακολουθήστε [τα εξής βήματα](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="3cea9-103">To search the Office 365 audit log, follow [these steps](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>

<span data-ttu-id="3cea9-104">**Ανταλλαγή**</span><span class="sxs-lookup"><span data-stu-id="3cea9-104">**Exchange**</span></span>

- <span data-ttu-id="3cea9-105">Δραστηριότητες διαχείρισης Exchange ελέγχονται από προεπιλογή.</span><span class="sxs-lookup"><span data-stu-id="3cea9-105">Exchange admin activities are audited by default.</span></span>

- <span data-ttu-id="3cea9-106">Είμαστε στη διαδικασία Ενεργοποίηση ελέγχου γραμματοκιβωτίου από προεπιλογή στο Office 365.</span><span class="sxs-lookup"><span data-stu-id="3cea9-106">We are in the process of enabling mailbox auditing by default in Office 365.</span></span> <span data-ttu-id="3cea9-107">Μέχρι τότε, για να ενεργοποιήσετε τον έλεγχο για ένα μόνο γραμματοκιβώτιο ή για όλα τα γραμματοκιβώτια στον οργανισμό σας, ανατρέξτε στην ενότητα [αυτού του άρθρου](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing).</span><span class="sxs-lookup"><span data-stu-id="3cea9-107">Until then, to enable auditing for a single mailbox or for all mailboxes in your organization, see  [this article](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing).</span></span>

- <span data-ttu-id="3cea9-108">Office 365 ομάδα γραμματοκιβώτια και δημόσιου φακέλου γραμματοκιβώτια στο Exchange Online δεν υποστηρίζει αρχεία καταγραφής ελέγχου.</span><span class="sxs-lookup"><span data-stu-id="3cea9-108">Office 365 Group mailboxes and public folder mailboxes in Exchange Online don't support audit logging.</span></span>

<span data-ttu-id="3cea9-109">**Του SharePoint και OneDrive**</span><span class="sxs-lookup"><span data-stu-id="3cea9-109">**SharePoint and OneDrive**</span></span>

- <span data-ttu-id="3cea9-110">Δεν υπάρχει καμία πρόσθετη ρύθμιση παραμέτρων που απαιτείται για να ενεργοποιήσετε τον έλεγχο του SharePoint και OneDrive.</span><span class="sxs-lookup"><span data-stu-id="3cea9-110">There's no additional configuration required to enable auditing for SharePoint and OneDrive.</span></span>

- <span data-ttu-id="3cea9-111">Του SharePoint και OneDrive υποστηρίζουν τον έλεγχο τους ακόλουθους τύπους δραστηριοτήτων:</span><span class="sxs-lookup"><span data-stu-id="3cea9-111">SharePoint and OneDrive support auditing the following types of activities:</span></span>

    - <span data-ttu-id="3cea9-112">Αρχείο, φάκελο και δραστηριότητες σελίδα</span><span class="sxs-lookup"><span data-stu-id="3cea9-112">File, folder, and page activities</span></span>
    - <span data-ttu-id="3cea9-113">Κοινή χρήση και πρόσβαση σε δραστηριότητες</span><span class="sxs-lookup"><span data-stu-id="3cea9-113">Sharing and access request activities</span></span>
    - <span data-ttu-id="3cea9-114">Δραστηριότητες διαχείρισης τοποθεσίας</span><span class="sxs-lookup"><span data-stu-id="3cea9-114">Site administration activities</span></span>
    - <span data-ttu-id="3cea9-115">Αρχείο δραστηριοτήτων συγχρονισμού</span><span class="sxs-lookup"><span data-stu-id="3cea9-115">File synchronization activities</span></span>

- <span data-ttu-id="3cea9-116">Για πληροφορίες σχετικά με δραστηριότητες ελέγχονται σε άλλες υπηρεσίες του Office 365, ανατρέξτε [στον πίνακα σε αυτό το άρθρο](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#audited-activities).</span><span class="sxs-lookup"><span data-stu-id="3cea9-116">For information about audited activities in other Office 365 services, see  [the table in this article](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#audited-activities).</span></span>

- <span data-ttu-id="3cea9-117">Εδώ μια λίστα με συνήθεις ερωτήσεις [συχνές ερωτήσεις](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#frequently-asked-questions) σχετικά με την αναζήτηση στο αρχείο καταγραφής ελέγχου.</span><span class="sxs-lookup"><span data-stu-id="3cea9-117">Here a list of frequently asked questions [frequently asked questions](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#frequently-asked-questions) about searching the audit log.</span></span>