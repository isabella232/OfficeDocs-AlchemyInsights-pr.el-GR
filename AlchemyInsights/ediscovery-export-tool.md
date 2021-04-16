---
title: Εργαλείο εξαγωγής eDiscovery
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: b1100175c75fb77a499e706380305eb016cf1b2b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814588"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a><span data-ttu-id="3d0ae-102">Δεν μπορείτε να εγκαταστήσετε ή να εκτελέσετε το Εργαλείο εξαγωγής eDiscovery;</span><span class="sxs-lookup"><span data-stu-id="3d0ae-102">Can't install or run the eDiscovery Export Tool?</span></span>

<span data-ttu-id="3d0ae-103">Εάν δεν μπορείτε να εγκαταστήσετε ή να εκτελέσετε το Εργαλείο εξαγωγής eDiscovery για να κάνετε λήψη των αποτελεσμάτων αναζήτησης, ελέγξτε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="3d0ae-103">If you can't install or run the eDiscovery Export Tool to download search results, check the following things:</span></span>
  
- <span data-ttu-id="3d0ae-104">Ο υπολογιστής που χρησιμοποιείτε πληροί τα εξής προαπαιτούμενα:</span><span class="sxs-lookup"><span data-stu-id="3d0ae-104">The computer you're using meets these pre-requisites:</span></span>

  - <span data-ttu-id="3d0ae-105">Εκδόσεις 32 ή 64 bit των Windows 7 και νεότερες εκδόσεις</span><span class="sxs-lookup"><span data-stu-id="3d0ae-105">32- or 64-bit versions of Windows 7 and later versions</span></span>

  - <span data-ttu-id="3d0ae-106">Microsoft .NET Framework 4.7</span><span class="sxs-lookup"><span data-stu-id="3d0ae-106">Microsoft .NET Framework 4.7</span></span>

  - <span data-ttu-id="3d0ae-107">Ένα υποστηριζόμενο πρόγραμμα περιήγησης:</span><span class="sxs-lookup"><span data-stu-id="3d0ae-107">A supported browser:</span></span>

  - <span data-ttu-id="3d0ae-108">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="3d0ae-108">Microsoft Edge</span></span>

    <span data-ttu-id="3d0ae-109">Ή</span><span class="sxs-lookup"><span data-stu-id="3d0ae-109">Or</span></span>

  - <span data-ttu-id="3d0ae-110">Internet Explorer 10 και νεότερες εκδόσεις</span><span class="sxs-lookup"><span data-stu-id="3d0ae-110">Internet Explorer 10 and later versions</span></span>

    <span data-ttu-id="3d0ae-111">Άλλα προγράμματα περιήγησης, όπως το Google Chrome και το Mozilla Firefox δεν υποστηρίζονται.</span><span class="sxs-lookup"><span data-stu-id="3d0ae-111">Other browsers, such as Google Chrome and Mozilla Firefox aren't supported.</span></span>

- <span data-ttu-id="3d0ae-112">Ο οργανισμός σας μπορεί να συνδεθεί με το τελικό σημείο στο Azure, το οποίο είναι **\* .blob.core.windows.net** (ο χαρακτήρες μπαλαντέρ αντιπροσωπεύει ένα μοναδικό αναγνωριστικό για την εργασία εξαγωγής).</span><span class="sxs-lookup"><span data-stu-id="3d0ae-112">Your organization can connect to the endpoint in Azure, which is **\*.blob.core.windows.net** (the wildcard represents a unique identifier for your export job).</span></span>

- <span data-ttu-id="3d0ae-113">Σας έχει εκχωρηθεί ο ρόλος "Εξαγωγή" στο Κέντρο συμμόρφωσης ασφαλείας του Microsoft &amp; 365.</span><span class="sxs-lookup"><span data-stu-id="3d0ae-113">You're assigned the Export role in the Microsoft 365 Security &amp; Compliance Center.</span></span> <span data-ttu-id="3d0ae-114">Από προεπιλογή, αυτός ο ρόλος εκχωρείται μόνο στην ομάδα ρόλων της Διαχείρισης eDiscovery.</span><span class="sxs-lookup"><span data-stu-id="3d0ae-114">By default, this role is only assigned to the eDiscovery Manager role group.</span></span> <span data-ttu-id="3d0ae-115">Ανατρέξτε [στο θέμα Εκχώρηση δικαιωμάτων eDiscovery.](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions)</span><span class="sxs-lookup"><span data-stu-id="3d0ae-115">See [Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span></span>

<span data-ttu-id="3d0ae-116">Για περισσότερες πληροφορίες, ανατρέξτε στο [θέμα "Εξαγωγή αποτελεσμάτων αναζήτησης περιεχομένου".](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)</span><span class="sxs-lookup"><span data-stu-id="3d0ae-116">For more information, see [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>

<span data-ttu-id="3d0ae-117">Εάν εξάγετε περισσότερα από 100K γραμματοκιβώτια, θα πρέπει να χρησιμοποιήσετε το ακόλουθο Powershell για να κάνετε λήψη των αποτελεσμάτων εξαγωγής: Εξαγωγή αποτελεσμάτων από περισσότερα από [100K γραμματοκιβώτια.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)</span><span class="sxs-lookup"><span data-stu-id="3d0ae-117">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>