---
title: Εξαγωγή αποτελεσμάτων eDiscovery/Content Search
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
- "3200003"
- "7221"
ms.openlocfilehash: b93377a33eebc7899041b684449e46caedb04415
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50482625"
---
# <a name="export-ediscoverycontent-search-results"></a><span data-ttu-id="96df6-102">Εξαγωγή αποτελεσμάτων eDiscovery/Content Search</span><span class="sxs-lookup"><span data-stu-id="96df6-102">Export eDiscovery/Content Search results</span></span>

<span data-ttu-id="96df6-103">Ίσως χρειαστεί να εξαγάγετε τα αποτελέσματα της αναζήτησης σε ένα αρχείο PST (από μήνυμα ηλεκτρονικού ταχυδρομείου) ή σε εγγενή έγγραφα του Office (από τοποθεσίες του SharePoint και του OneDrive για επιχειρήσεις).</span><span class="sxs-lookup"><span data-stu-id="96df6-103">You may need to export your search results to a PST file (from email) or to native Office documents (from SharePoint and OneDrive for Business sites).</span></span> <span data-ttu-id="96df6-104">Εάν ναι, κάντε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="96df6-104">If so, do the following:</span></span>

- <span data-ttu-id="96df6-105">Βεβαιωθείτε ότι στο λογαριασμό σας έχουν εκχωρηθεί τα κατάλληλα δικαιώματα για εξαγωγή.</span><span class="sxs-lookup"><span data-stu-id="96df6-105">Make sure your account is assigned the proper permissions to export.</span></span> <span data-ttu-id="96df6-106">Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα Εκχώρηση δικαιώματος eDiscovery.](https://go.microsoft.com/fwlink/?linkid=2102406)</span><span class="sxs-lookup"><span data-stu-id="96df6-106">For more info, see [Assign eDiscovery permission](https://go.microsoft.com/fwlink/?linkid=2102406).</span></span>
- <span data-ttu-id="96df6-107">Βεβαιωθείτε ότι ο υπολογιστής σας έχει πληρούνται όλες τις [προϋποθέσεις.](https://docs.microsoft.com/office365/securitycompliance/export-search-results#before-you-begin)</span><span class="sxs-lookup"><span data-stu-id="96df6-107">Make sure your computer has met all [prerequisites](https://docs.microsoft.com/office365/securitycompliance/export-search-results#before-you-begin).</span></span> <span data-ttu-id="96df6-108">Δεν υποστηρίζονται όλα τα προγράμματα περιήγησης, όπως το Chrome.</span><span class="sxs-lookup"><span data-stu-id="96df6-108">Not all browsers are supported, such as Chrome.</span></span>
- <span data-ttu-id="96df6-109">Για εξαγωγή από μια αναζήτηση περιεχομένου: α.</span><span class="sxs-lookup"><span data-stu-id="96df6-109">To export from a Content Search: a.</span></span> <span data-ttu-id="96df6-110">Μεταβείτε στο Κέντρο [συμμόρφωσης &, κάντε](https://protection.office.com/contentsearch) κλικ στην επιλογή **"Αναζήτηση"** και, στη συνέχεια, **επιλέξτε "Αναζήτηση περιεχομένου".**</span><span class="sxs-lookup"><span data-stu-id="96df6-110">Go to the [Security & Compliance Center](https://protection.office.com/contentsearch) and click **Search**, and then select **Content search**.</span></span> <span data-ttu-id="96df6-111">Στη σελίδα **"Αναζήτηση περιεχομένου",** επιλέξτε μια αποθηκευμένη αναζήτηση.</span><span class="sxs-lookup"><span data-stu-id="96df6-111">On the **Content search** page, select a saved search.</span></span>
    <span data-ttu-id="96df6-112">b.</span><span class="sxs-lookup"><span data-stu-id="96df6-112">b.</span></span> <span data-ttu-id="96df6-113">Στο παράθυρο "Λεπτομέρειες", στην περιοχή **"Εξαγωγή αποτελεσμάτων σε υπολογιστή", επιλέξτε** **"Έναρξη εξαγωγής".**</span><span class="sxs-lookup"><span data-stu-id="96df6-113">On the Details pane, under **Export results to a computer**, select **Start export**.</span></span> <span data-ttu-id="96df6-114">Εάν εξάγετε περισσότερα από 100K γραμματοκιβώτια, θα πρέπει να χρησιμοποιήσετε το PowerShell για να κάνετε λήψη των αποτελεσμάτων εξαγωγής.</span><span class="sxs-lookup"><span data-stu-id="96df6-114">If you're exporting more than 100K mailboxes, you'll need to use PowerShell to download the export results.</span></span> <span data-ttu-id="96df6-115">Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα Εξαγωγή αποτελεσμάτων από περισσότερα από 100K γραμματοκιβώτια.](https://go.microsoft.com/fwlink/?linkid=2143861)</span><span class="sxs-lookup"><span data-stu-id="96df6-115">For more info, see [Exporting results from more than 100K mailboxes](https://go.microsoft.com/fwlink/?linkid=2143861).</span></span>

<span data-ttu-id="96df6-116">Για να μάθετε περισσότερα, ανατρέξτε [στο θέμα "Εξαγωγή αποτελεσμάτων αναζήτησης περιεχομένου".](https://go.microsoft.com/fwlink/?linkid=2102118)</span><span class="sxs-lookup"><span data-stu-id="96df6-116">To learn more, see [Export Content Search Results](https://go.microsoft.com/fwlink/?linkid=2102118).</span></span>