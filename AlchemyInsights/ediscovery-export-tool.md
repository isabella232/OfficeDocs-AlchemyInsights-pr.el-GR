---
title: εργαλείο εξαγωγής ανακάλυψης
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: 67e59182a5053111a08f5fb2be814931a1aa815d
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277937"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a><span data-ttu-id="a6395-102">Δεν μπορείτε να εγκαταστήσετε ή να εκτελέσετε το εργαλείο εξαγωγής ανακάλυψης;</span><span class="sxs-lookup"><span data-stu-id="a6395-102">Can't install or run the eDiscovery Export Tool?</span></span>

<span data-ttu-id="a6395-103">Εάν δεν μπορείτε να εγκαταστήσετε ή να εκτελέσετε το εργαλείο εξαγωγής ανακάλυψης για να κάνετε λήψη των αποτελεσμάτων αναζήτησης, ανατρέξτε στα παρακάτω στοιχεία:</span><span class="sxs-lookup"><span data-stu-id="a6395-103">If you can't install or run the eDiscovery Export Tool to download search results, check the following things:</span></span>
  
- <span data-ttu-id="a6395-104">Ο υπολογιστής που χρησιμοποιείτε πληροί αυτές τις προϋποθέσεις:</span><span class="sxs-lookup"><span data-stu-id="a6395-104">The computer you're using meets these pre-requisites:</span></span>

  - <span data-ttu-id="a6395-105">εκδόσεις 32 ή 64-bit των Windows 7 και των νεότερων εκδόσεων</span><span class="sxs-lookup"><span data-stu-id="a6395-105">32- or 64-bit versions of Windows 7 and later versions</span></span>

  - <span data-ttu-id="a6395-106">Microsoft .NET Framework 4.7</span><span class="sxs-lookup"><span data-stu-id="a6395-106">Microsoft .NET Framework 4.7</span></span>

  - <span data-ttu-id="a6395-107">Ένα υποστηριζόμενο πρόγραμμα περιήγησης:</span><span class="sxs-lookup"><span data-stu-id="a6395-107">A supported browser:</span></span>

  - <span data-ttu-id="a6395-108">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="a6395-108">Microsoft Edge</span></span>

    <span data-ttu-id="a6395-109">Ή</span><span class="sxs-lookup"><span data-stu-id="a6395-109">Or</span></span>

  - <span data-ttu-id="a6395-110">Internet Explorer 10 και νεότερες εκδόσεις</span><span class="sxs-lookup"><span data-stu-id="a6395-110">Internet Explorer 10 and later versions</span></span>

    <span data-ttu-id="a6395-111">Άλλα προγράμματα περιήγησης, όπως το Google Chrome και το Mozilla Firefox δεν υποστηρίζονται.</span><span class="sxs-lookup"><span data-stu-id="a6395-111">Other browsers, such as Google Chrome and Mozilla Firefox aren't supported.</span></span>

- <span data-ttu-id="a6395-112">Ο οργανισμός σας μπορεί να συνδεθεί με το τελικό σημείο στο Azure, το οποίο είναι \*\* \* . blob.Core.Windows.NET\*\* (ο χαρακτήρας μπαλαντέρ αντιπροσωπεύει ένα μοναδικό αναγνωριστικό για την εργασία εξαγωγής).</span><span class="sxs-lookup"><span data-stu-id="a6395-112">Your organization can connect to the endpoint in Azure, which is **\*.blob.core.windows.net** (the wildcard represents a unique identifier for your export job).</span></span>

- <span data-ttu-id="a6395-113">Σας έχει εκχωρηθεί ο ρόλος εξαγωγής στο κέντρο συμμόρφωσης ασφαλείας του Microsoft 365 &amp; .</span><span class="sxs-lookup"><span data-stu-id="a6395-113">You're assigned the Export role in the Microsoft 365 Security &amp; Compliance Center.</span></span> <span data-ttu-id="a6395-114">Από προεπιλογή, αυτός ο ρόλος εκχωρείται μόνο στην ομάδα ρόλων της διαχείρισης ανακάλυψης.</span><span class="sxs-lookup"><span data-stu-id="a6395-114">By default, this role is only assigned to the eDiscovery Manager role group.</span></span> <span data-ttu-id="a6395-115">Ανατρέξτε στο θέμα [εκχώρηση δικαιωμάτων ανακάλυψης](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span><span class="sxs-lookup"><span data-stu-id="a6395-115">See [Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span></span>

<span data-ttu-id="a6395-116">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Εξαγωγή αποτελεσμάτων αναζήτησης περιεχομένου](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span><span class="sxs-lookup"><span data-stu-id="a6395-116">For more information, see [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>

<span data-ttu-id="a6395-117">Εάν εξάγετε περισσότερα από 100K γραμματοκιβώτια, θα πρέπει να χρησιμοποιήσετε το ακόλουθο PowerShell για να κάνετε λήψη των αποτελεσμάτων εξαγωγής:  [Εξαγωγή αποτελεσμάτων από περισσότερα από 100K γραμματοκιβώτια](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="a6395-117">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>