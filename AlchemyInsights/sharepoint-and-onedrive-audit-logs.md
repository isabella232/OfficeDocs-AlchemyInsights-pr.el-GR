---
title: Κλασικές αναφορές καταγραφής ελέγχου του SharePoint
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: be95034bea3c58a4fde96cfb0f9ba525e810758e
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37992618"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="dbba1-102">Αρχεία καταγραφής ελέγχου του SharePoint και του OneDrive</span><span class="sxs-lookup"><span data-stu-id="dbba1-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="dbba1-103">Κλασικά αρχεία καταγραφής ελέγχου του SharePoint</span><span class="sxs-lookup"><span data-stu-id="dbba1-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="dbba1-104">Ο έλεγχος παλαιού τύπου, μεταφέρθηκε στο Ενοποιημένο αρχείο καταγραφής ελέγχου.</span><span class="sxs-lookup"><span data-stu-id="dbba1-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="dbba1-105">Όλες οι αναφορές παλαιού τύπου λογιστικού ελέγχου θα τροφοδοτηθεί τώρα μέσω ΝΟΑ, και τα παλαιά σήματα ελέγχου έχουν μετεγκατασταθεί σε ΝΟΑ.</span><span class="sxs-lookup"><span data-stu-id="dbba1-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="dbba1-106">Βασικές αλλαγές:</span><span class="sxs-lookup"><span data-stu-id="dbba1-106">Key changes:</span></span>

* <span data-ttu-id="dbba1-107">Η περικοπή δεν είναι διαθέσιμη ως δυνατότητα.</span><span class="sxs-lookup"><span data-stu-id="dbba1-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="dbba1-108">Η επιλογή συγκεκριμένων συμβάντων για έλεγχο δεν είναι διαθέσιμη.</span><span class="sxs-lookup"><span data-stu-id="dbba1-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="dbba1-109">Ανατρέξτε σε [αυτό το έγγραφο](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) για μια πλήρη λίστα των ελεγχθέντων συμβάντων που είναι διαθέσιμα από προεπιλογή.</span><span class="sxs-lookup"><span data-stu-id="dbba1-109">Refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="dbba1-110">Η επιλογή **θέσης** στην περιοχή **προσαρμοσμένες αναφορές** δεν είναι διαθέσιμη.</span><span class="sxs-lookup"><span data-stu-id="dbba1-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="dbba1-111">Η επιλογή συμβάντα **ανοίγματος ή λήψης εγγράφων** δεν είναι διαθέσιμη.</span><span class="sxs-lookup"><span data-stu-id="dbba1-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="dbba1-112">Ρύθμιση παραμέτρων ελέγχου για μια συλλογή τοποθεσιών</span><span class="sxs-lookup"><span data-stu-id="dbba1-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="dbba1-113">SharePoint και OneDrive σύγχρονο Ενοποιημένο ελέγχου αρχεία καταγραφής από τη συμμόρφωση</span><span class="sxs-lookup"><span data-stu-id="dbba1-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="dbba1-114">Ενεργοποίηση/απενεργοποίηση ενοποιημένης καταγραφής ελέγχου</span><span class="sxs-lookup"><span data-stu-id="dbba1-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="dbba1-115">Δεν απαιτείται επιπλέον ρύθμιση παραμέτρων στο SharePoint ή στο OneDrive.</span><span class="sxs-lookup"><span data-stu-id="dbba1-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="dbba1-116">Χρησιμοποιήστε την αναζήτηση καταγραφής ελέγχου για να ελέγξετε τη δραστηριότητα των αρχείων, των φακέλων, των χρηστών, των δικαιωμάτων:</span><span class="sxs-lookup"><span data-stu-id="dbba1-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="dbba1-117">Δραστηριότητες αρχείων και σελίδων</span><span class="sxs-lookup"><span data-stu-id="dbba1-117">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="dbba1-118">Δραστηριότητες φακέλων</span><span class="sxs-lookup"><span data-stu-id="dbba1-118">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="dbba1-119">Δραστηριότητες αίτησης κοινής χρήσης και πρόσβασης</span><span class="sxs-lookup"><span data-stu-id="dbba1-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="dbba1-120">Δραστηριότητες συγχρονισμού</span><span class="sxs-lookup"><span data-stu-id="dbba1-120">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="dbba1-121">Δραστηριότητες διαχείρισης τοποθεσίας</span><span class="sxs-lookup"><span data-stu-id="dbba1-121">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="dbba1-122">Για περισσότερες πληροφορίες σχετικά με τον τρόπο ανάκτησης αυτών των συμβάντων, ανατρέξτε [στο θέμα Αναζήτηση στο αρχείο καταγραφής ελέγχου](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="dbba1-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
