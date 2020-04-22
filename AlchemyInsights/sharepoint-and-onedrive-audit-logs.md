---
title: Κλασικές αναφορές αρχείου καταγραφής ελέγχου του SharePoint
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 3270f1ab03bacb235cbdc3d710053c858f0a5183
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741965"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="0305e-102">Αρχεία καταγραφής ελέγχου του SharePoint και του OneDrive</span><span class="sxs-lookup"><span data-stu-id="0305e-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="0305e-103">Κλασικά αρχεία καταγραφής ελέγχου του SharePoint</span><span class="sxs-lookup"><span data-stu-id="0305e-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="0305e-104">Ο έλεγχος παλαιού τύπου SPO μετεγκαταστάθηκε στο ενοποιημένο αρχείο καταγραφής ελέγχου (UAL).</span><span class="sxs-lookup"><span data-stu-id="0305e-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="0305e-105">Όλες οι αναφορές ελέγχου παλαιού τύπου SPO θα τροφοδοτούνται τώρα μέσω UAL και τα σήματα ελέγχου παλαιού τύπου έχουν μετεγκατασταθεί σε UAL.</span><span class="sxs-lookup"><span data-stu-id="0305e-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="0305e-106">Βασικές αλλαγές:</span><span class="sxs-lookup"><span data-stu-id="0305e-106">Key changes:</span></span>

* <span data-ttu-id="0305e-107">Η περικοπή ΔΕΝ είναι διαθέσιμη ως δυνατότητα.</span><span class="sxs-lookup"><span data-stu-id="0305e-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="0305e-108">Η επιλογή συγκεκριμένων συμβάντων για έλεγχο ΔΕΝ είναι διαθέσιμη.</span><span class="sxs-lookup"><span data-stu-id="0305e-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="0305e-109">Ανατρέξτε σε [αυτό το έγγραφο](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) για μια πλήρη λίστα των ελεγμένα συμβάντα που είναι διαθέσιμα από προεπιλογή.</span><span class="sxs-lookup"><span data-stu-id="0305e-109">Refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="0305e-110">Η **επιλογή "Θέση"** στην περιοχή **Προσαρμοσμένες αναφορές** ΔΕΝ είναι διαθέσιμη.</span><span class="sxs-lookup"><span data-stu-id="0305e-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="0305e-111">Η επιλογή **Άνοιγμα ή λήψη συμβάντων εγγράφων** ΔΕΝ είναι διαθέσιμη.</span><span class="sxs-lookup"><span data-stu-id="0305e-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="0305e-112">Ρύθμιση παραμέτρων ελέγχου για μια συλλογή τοποθεσιών</span><span class="sxs-lookup"><span data-stu-id="0305e-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="0305e-113">Αρχεία καταγραφής ενοποιημένου ελέγχου του SharePoint και του OneDrive (Unified Audit) του SharePoint και του OneDrive</span><span class="sxs-lookup"><span data-stu-id="0305e-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="0305e-114">Ενεργοποίηση/απενεργοποίηση ενοποιημένης καταγραφής ελέγχου</span><span class="sxs-lookup"><span data-stu-id="0305e-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="0305e-115">Δεν απαιτείται πρόσθετη ρύθμιση παραμέτρων στο SharePoint ή το OneDrive.</span><span class="sxs-lookup"><span data-stu-id="0305e-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="0305e-116">Χρησιμοποιήστε την αναζήτηση καταγραφής ελέγχου για να ελέγξετε τη δραστηριότητα των αρχείων, φακέλων, χρηστών, δικαιωμάτων:</span><span class="sxs-lookup"><span data-stu-id="0305e-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="0305e-117">Δραστηριότητες αρχείων και σελίδων</span><span class="sxs-lookup"><span data-stu-id="0305e-117">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="0305e-118">Δραστηριότητες φακέλων</span><span class="sxs-lookup"><span data-stu-id="0305e-118">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="0305e-119">Δραστηριότητες κοινής χρήσης και αίτησης πρόσβασης</span><span class="sxs-lookup"><span data-stu-id="0305e-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="0305e-120">Δραστηριότητες συγχρονισμού</span><span class="sxs-lookup"><span data-stu-id="0305e-120">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="0305e-121">Δραστηριότητες διαχείρισης τοποθεσίας</span><span class="sxs-lookup"><span data-stu-id="0305e-121">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="0305e-122">Για περισσότερες πληροφορίες σχετικά με τον τρόπο ανάκτησης αυτών των συμβάντων, ανατρέξτε στο θέμα [Αναζήτηση στο αρχείο καταγραφής ελέγχου](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="0305e-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
