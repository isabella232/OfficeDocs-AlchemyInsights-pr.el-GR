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
ms.openlocfilehash: af5b3c76b82db13bc89c917247e41fa1d8779b68
ms.sourcegitcommit: d5bf97a0bf0547f36b6da9684ce9f16a13a7749e
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/20/2019
ms.locfileid: "37068023"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="55315-102">Αρχεία καταγραφής ελέγχου του SharePoint και του OneDrive</span><span class="sxs-lookup"><span data-stu-id="55315-102">SharePoint and OneDrive audit logs</span></span>

<span data-ttu-id="55315-103">**SharePoint και OneDrive σύγχρονο Ενοποιημένο ελέγχου αρχεία καταγραφής από τη συμμόρφωση**</span><span class="sxs-lookup"><span data-stu-id="55315-103">**SharePoint and OneDrive Modern Unified Audit logs from compliance**</span></span>

- [<span data-ttu-id="55315-104">Ενεργοποίηση/απενεργοποίηση ενοποιημένης καταγραφής ελέγχου</span><span class="sxs-lookup"><span data-stu-id="55315-104">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="55315-105">Δεν απαιτείται επιπλέον ρύθμιση παραμέτρων στο SharePoint ή στο OneDrive.</span><span class="sxs-lookup"><span data-stu-id="55315-105">No additional configuration is required within SharePoint or OneDrive.</span></span>

- <span data-ttu-id="55315-106">Χρησιμοποιήστε την αναζήτηση καταγραφής ελέγχου για να ελέγξετε τη δραστηριότητα των αρχείων, των φακέλων, των χρηστών, των δικαιωμάτων:</span><span class="sxs-lookup"><span data-stu-id="55315-106">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

    - [<span data-ttu-id="55315-107">Δραστηριότητες αρχείων και σελίδων</span><span class="sxs-lookup"><span data-stu-id="55315-107">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
    - [<span data-ttu-id="55315-108">Δραστηριότητες φακέλων</span><span class="sxs-lookup"><span data-stu-id="55315-108">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    - [<span data-ttu-id="55315-109">Δραστηριότητες αίτησης κοινής χρήσης και πρόσβασης</span><span class="sxs-lookup"><span data-stu-id="55315-109">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
    - [<span data-ttu-id="55315-110">Δραστηριότητες συγχρονισμού</span><span class="sxs-lookup"><span data-stu-id="55315-110">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
    - [<span data-ttu-id="55315-111">Δραστηριότητες διαχείρισης τοποθεσίας</span><span class="sxs-lookup"><span data-stu-id="55315-111">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)
- <span data-ttu-id="55315-112">Για περισσότερες πληροφορίες σχετικά με τον τρόπο ανάκτησης αυτών των συμβάντων, ανατρέξτε [στο θέμα Αναζήτηση στο αρχείο καταγραφής ελέγχου](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="55315-112">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>

<span data-ttu-id="55315-113">**Κλασικά αρχεία καταγραφής ελέγχου του SharePoint**</span><span class="sxs-lookup"><span data-stu-id="55315-113">**SharePoint classic Audit logs**</span></span>

<span data-ttu-id="55315-114">Μετανάστευσα παλαιού τύπου λογιστικό έλεγχο σε ενοποιημένο αρχείο καταγραφής ελέγχου (δι).</span><span class="sxs-lookup"><span data-stu-id="55315-114">We migrated SPO legacy auditing to Unified Audit Log (UAL).</span></span> <span data-ttu-id="55315-115">Αυτό ουσιαστικά σημαίνει ότι όλες οι αναφορές παλαιού τύπου λογιστικού ελέγχου θα τροφοδοτηθεί τώρα μέσω του ΝΟΑ, και τα παλαιότερα σήματα ελέγχου έχουν μεταφερθεί στο ΝΟΑ.</span><span class="sxs-lookup"><span data-stu-id="55315-115">This essentially means that all SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="55315-116">Βασικές αλλαγές:</span><span class="sxs-lookup"><span data-stu-id="55315-116">Key changes:</span></span>

- <span data-ttu-id="55315-117">Η περικοπή ως δυνατότητα δεν είναι διαθέσιμη.</span><span class="sxs-lookup"><span data-stu-id="55315-117">Trimming as a capability is NOT available.</span></span>
- <span data-ttu-id="55315-118">Η ενότητα όπου επιλέγετε συγκεκριμένα συμβάντα για έλεγχο δεν είναι διαθέσιμη.</span><span class="sxs-lookup"><span data-stu-id="55315-118">The section where you choose specific events to audit is NOT available.</span></span> <span data-ttu-id="55315-119">Ανατρέξτε σε [αυτό το έγγραφο](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) για μια πλήρη λίστα των ελεγχθέντων συμβάντων που είναι διαθέσιμα από προεπιλογή.</span><span class="sxs-lookup"><span data-stu-id="55315-119">Please refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
- <span data-ttu-id="55315-120">Η επιλογή "τοποθεσία" κάτω από τις **προσαρμοσμένες ΑΝΑΦΟΡΈς** δεν είναι διαθέσιμη.</span><span class="sxs-lookup"><span data-stu-id="55315-120">The "Location" option under **Customized reports** is NOT available.</span></span> 
- <span data-ttu-id="55315-121">Τα συμβάντα "Άνοιγμα ή λήψη εγγράφων" δεν είναι διαθέσιμα.</span><span class="sxs-lookup"><span data-stu-id="55315-121">“Opening or downloading documents” events is NOT available.</span></span> 

