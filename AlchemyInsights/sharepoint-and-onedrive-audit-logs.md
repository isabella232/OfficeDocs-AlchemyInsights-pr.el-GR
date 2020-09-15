---
title: Κλασικές αναφορές αρχείου καταγραφής ελέγχου του SharePoint
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: daf79f8d75ccdff8ad54f0f307648a5832a6bb71
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662208"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="4468a-102">Αρχεία καταγραφής ελέγχου του SharePoint και του OneDrive</span><span class="sxs-lookup"><span data-stu-id="4468a-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="4468a-103">Αρχεία καταγραφής ελέγχου του SharePoint Classic</span><span class="sxs-lookup"><span data-stu-id="4468a-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="4468a-104">Ο έλεγχος παλαιού τύπου SPO μετεγκαταστάθηκε σε ενοποιημένο αρχείο καταγραφής ελέγχου (UAL).</span><span class="sxs-lookup"><span data-stu-id="4468a-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="4468a-105">Όλες οι αναφορές ελέγχου παλαιού τύπου SPO θα τροφοδοτούνται πλέον μέσω του UAL και τα σήματα ελέγχου παλαιού τύπου έχουν μετεγκατασταθεί στο UAL.</span><span class="sxs-lookup"><span data-stu-id="4468a-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="4468a-106">Βασικές αλλαγές:</span><span class="sxs-lookup"><span data-stu-id="4468a-106">Key changes:</span></span>

* <span data-ttu-id="4468a-107">Η περικοπή δεν είναι διαθέσιμη ως δυνατότητα.</span><span class="sxs-lookup"><span data-stu-id="4468a-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="4468a-108">Η επιλογή συγκεκριμένων συμβάντων για έλεγχο δεν είναι διαθέσιμη.</span><span class="sxs-lookup"><span data-stu-id="4468a-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="4468a-109">Ανατρέξτε σε [αυτό το έγγραφο](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) για μια πλήρη λίστα των ελεγμένων συμβάντων που είναι διαθέσιμα από προεπιλογή.</span><span class="sxs-lookup"><span data-stu-id="4468a-109">Refer to [this document](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="4468a-110">Η επιλογή " **θέση** " στην περιοχή " **ΠΡΟΣΑΡΜΟΣΜΈΝΕς αναφορές** " δεν είναι διαθέσιμη.</span><span class="sxs-lookup"><span data-stu-id="4468a-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="4468a-111">Η επιλογή " **Άνοιγμα ή λήψη συμβάντων εγγράφων** " δεν είναι διαθέσιμη.</span><span class="sxs-lookup"><span data-stu-id="4468a-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="4468a-112">Ρύθμιση παραμέτρων των ρυθμίσεων ελέγχου για μια συλλογή τοποθεσιών</span><span class="sxs-lookup"><span data-stu-id="4468a-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="4468a-113">Αρχεία καταγραφής σύγχρονων ενοποιημένων ελέγχων του SharePoint και του OneDrive από τη συμμόρφωση</span><span class="sxs-lookup"><span data-stu-id="4468a-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="4468a-114">Ενεργοποίηση/απενεργοποίηση της ενοποιημένης καταγραφής ελέγχου</span><span class="sxs-lookup"><span data-stu-id="4468a-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="4468a-115">Δεν απαιτείται πρόσθετη ρύθμιση παραμέτρων μέσα από το SharePoint ή το OneDrive.</span><span class="sxs-lookup"><span data-stu-id="4468a-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="4468a-116">Χρησιμοποιήστε την αναζήτηση καταγραφής ελέγχου για να ελέγξετε τη δραστηριότητα των αρχείων, των φακέλων ή των χρηστών, των δικαιωμάτων:</span><span class="sxs-lookup"><span data-stu-id="4468a-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="4468a-117">Δραστηριότητες αρχείων και σελίδων</span><span class="sxs-lookup"><span data-stu-id="4468a-117">File and page activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="4468a-118">Δραστηριότητες φακέλου</span><span class="sxs-lookup"><span data-stu-id="4468a-118">Folder activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="4468a-119">Δραστηριότητες αίτησης για κοινή χρήση και πρόσβαση</span><span class="sxs-lookup"><span data-stu-id="4468a-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="4468a-120">Δραστηριότητες συγχρονισμού</span><span class="sxs-lookup"><span data-stu-id="4468a-120">Synchronization activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="4468a-121">Δραστηριότητες διαχείρισης τοποθεσίας</span><span class="sxs-lookup"><span data-stu-id="4468a-121">Site administration activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="4468a-122">Για περισσότερες πληροφορίες σχετικά με τον τρόπο ανάκτησης αυτών των συμβάντων, ανατρέξτε [στο θέμα Αναζήτηση στο αρχείο καταγραφής ελέγχου](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="4468a-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
