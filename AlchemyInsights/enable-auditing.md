---
title: Έλεγχος 286-ενεργοποίηση
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 286
ms.assetid: ''
ms.openlocfilehash: 4f5829ac1ecc7d01575df360929d1a775e626e2a
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32398926"
---
# <a name="search-the-audit-log"></a><span data-ttu-id="d7339-102">Αναζήτηση στο αρχείο καταγραφής ελέγχου</span><span class="sxs-lookup"><span data-stu-id="d7339-102">Search the audit log</span></span>

<span data-ttu-id="d7339-103">Για να αναζητήσετε το αρχείο καταγραφής ελέγχου του Office 365, ακολουθήστε [τα εξής βήματα](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="d7339-103">To search the Office 365 audit log, follow [these steps](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span> 

<span data-ttu-id="d7339-104">**Ανταλλαγή**</span><span class="sxs-lookup"><span data-stu-id="d7339-104">**Exchange**</span></span>

- <span data-ttu-id="d7339-105">Δραστηριότητες διαχείρισης Exchange ελέγχονται από προεπιλογή.</span><span class="sxs-lookup"><span data-stu-id="d7339-105">Exchange admin activities are audited by default.</span></span>

- <span data-ttu-id="d7339-106">Είμαστε στη διαδικασία Ενεργοποίηση ελέγχου γραμματοκιβωτίου από προεπιλογή στο Office 365.</span><span class="sxs-lookup"><span data-stu-id="d7339-106">We are in the process of enabling mailbox auditing by default in Office 365.</span></span> <span data-ttu-id="d7339-107">Μέχρι τότε, για να ενεργοποιήσετε τον έλεγχο για ένα μόνο γραμματοκιβώτιο ή για όλα τα γραμματοκιβώτια στον οργανισμό σας, ανατρέξτε στην ενότητα [αυτού του άρθρου](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing).</span><span class="sxs-lookup"><span data-stu-id="d7339-107">Until then, to enable auditing for a single mailbox or for all mailboxes in your organization, see  [this article](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing).</span></span>

- <span data-ttu-id="d7339-108">Office 365 ομάδα γραμματοκιβώτια και δημόσιου φακέλου γραμματοκιβώτια στο Exchange Online δεν υποστηρίζει αρχεία καταγραφής ελέγχου.</span><span class="sxs-lookup"><span data-stu-id="d7339-108">Office 365 Group mailboxes and public folder mailboxes in Exchange Online don't support audit logging.</span></span>

<span data-ttu-id="d7339-109">**Του SharePoint και OneDrive**</span><span class="sxs-lookup"><span data-stu-id="d7339-109">**SharePoint and OneDrive**</span></span>

- <span data-ttu-id="d7339-110">Δεν υπάρχει καμία πρόσθετη ρύθμιση παραμέτρων που απαιτείται για να ενεργοποιήσετε τον έλεγχο του SharePoint και OneDrive.</span><span class="sxs-lookup"><span data-stu-id="d7339-110">There's no additional configuration required to enable auditing for SharePoint and OneDrive.</span></span>

- <span data-ttu-id="d7339-111">Του SharePoint και OneDrive υποστηρίζουν τον έλεγχο τους ακόλουθους τύπους δραστηριοτήτων:</span><span class="sxs-lookup"><span data-stu-id="d7339-111">SharePoint and OneDrive support auditing the following types of activities:</span></span> 

    - <span data-ttu-id="d7339-112">Αρχείο, φάκελο και δραστηριότητες σελίδα</span><span class="sxs-lookup"><span data-stu-id="d7339-112">File, folder, and page activities</span></span>
    - <span data-ttu-id="d7339-113">Κοινή χρήση και πρόσβαση σε δραστηριότητες</span><span class="sxs-lookup"><span data-stu-id="d7339-113">Sharing and access request activities</span></span>
    - <span data-ttu-id="d7339-114">Δραστηριότητες διαχείρισης τοποθεσίας</span><span class="sxs-lookup"><span data-stu-id="d7339-114">Site administration activities</span></span>
    - <span data-ttu-id="d7339-115">Αρχείο δραστηριοτήτων συγχρονισμού</span><span class="sxs-lookup"><span data-stu-id="d7339-115">File synchronization activities</span></span>

- <span data-ttu-id="d7339-116">Για πληροφορίες σχετικά με δραστηριότητες ελέγχονται σε άλλες υπηρεσίες του Office 365, ανατρέξτε [στον πίνακα σε αυτό το άρθρο](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#audited-activities).</span><span class="sxs-lookup"><span data-stu-id="d7339-116">For information about audited activities in other Office 365 services, see  [the table in this article](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#audited-activities).</span></span>

- <span data-ttu-id="d7339-117">Εδώ μια λίστα με συνήθεις ερωτήσεις [συχνές ερωτήσεις](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#frequently-asked-questions) σχετικά με την αναζήτηση στο αρχείο καταγραφής ελέγχου.</span><span class="sxs-lookup"><span data-stu-id="d7339-117">Here a list of frequently asked questions [frequently asked questions](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#frequently-asked-questions) about searching the audit log.</span></span>