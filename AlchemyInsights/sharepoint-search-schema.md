---
title: Διαχείριση σχήματος αναζήτησης στο SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 9836cf139e97fc556995a8f0ad38c51c5c2392ac
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40042963"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="cfcd8-102">Διαχείριση σχήματος αναζήτησης στο SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="cfcd8-102">Manage search schema in SharePoint Online</span></span>

<span data-ttu-id="cfcd8-103">Το σχήμα αναζήτησης ελέγχει τι μπορούν να αναζητήσουν οι χρήστες, πώς μπορούν οι χρήστες να το αναζητήσουν και πώς μπορείτε να παρουσιάσετε τα αποτελέσματα στις τοποθεσίες Web αναζήτησης.</span><span class="sxs-lookup"><span data-stu-id="cfcd8-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="cfcd8-104">Ανατρέξτε στο [πλαίσιο διαχείριση του σχήματος αναζήτησης στο SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) για να μάθετε πώς να:</span><span class="sxs-lookup"><span data-stu-id="cfcd8-104">See [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) to learn how to:</span></span> 
- <span data-ttu-id="cfcd8-105">Αλλάξτε το σχήμα αναζήτησης.</span><span class="sxs-lookup"><span data-stu-id="cfcd8-105">Change the search schema.</span></span>
- <span data-ttu-id="cfcd8-106">Δημιουργία διαχειριζόμενων ιδιοτήτων.</span><span class="sxs-lookup"><span data-stu-id="cfcd8-106">Create managed properties.</span></span>
- <span data-ttu-id="cfcd8-107">Οι ανιχνευμένες ιδιότητες του χάρτη ανιχνεύθηκαν σε διαχειριζόμενες ιδιότητες.</span><span class="sxs-lookup"><span data-stu-id="cfcd8-107">Map crawled map crawled properties to managed properties.</span></span>

<span data-ttu-id="cfcd8-108">Σημειώστε τα εξής όσον αφορά τη διαχείριση του σχήματος αναζήτησης:</span><span class="sxs-lookup"><span data-stu-id="cfcd8-108">Note the following in regards to managing your Search Schema:</span></span>

- <span data-ttu-id="cfcd8-109">Εάν λάβετε μια προειδοποίηση που αναφέρει ότι **η εφαρμογή έχει διακοπεί κατά την** πραγματοποίηση μιας αλλαγής σχήματος, αυτό είναι μόνο προσωρινό, καθώς υπάρχει συντήρηση υπηρεσίας που παρουσιάζεται.</span><span class="sxs-lookup"><span data-stu-id="cfcd8-109">If you receive a warning stating **the application is paused** when making a schema change, this is only temporary as there is service maintenance occurring.</span></span> 

    <span data-ttu-id="cfcd8-110">Εάν έχουν περάσει περισσότερες από 24 ώρες και εξακολουθείτε να αντιμετωπίζετε την προειδοποίηση, παρακαλούμε να καταγράψετε μια υπόθεση υποστήριξης.</span><span class="sxs-lookup"><span data-stu-id="cfcd8-110">If more than 24 hours have passed and you still experience the warning, please log a support case.</span></span>
- <span data-ttu-id="cfcd8-111">Όταν αλλάζετε τις διαχειριζόμενες ιδιότητες ή προσθέτετε νέες, οι αλλαγές ισχύουν μόνο μετά την επαναανίχνευση του περιεχομένου.</span><span class="sxs-lookup"><span data-stu-id="cfcd8-111">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="cfcd8-112">Στο SharePoint Online, η ανίχνευση συμβαίνει αυτόματα με βάση το καθορισμένο πρόγραμμα ανίχνευσης.</span><span class="sxs-lookup"><span data-stu-id="cfcd8-112">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>
- <span data-ttu-id="cfcd8-113">Για να βεβαιωθείτε ότι οι αλλαγές σας ανιχνεύθηκαν, μπορείτε να [ζητήσετε συγκεκριμένα μια επαναευρετηριοποίηση της λίστας ή της βιβλιοθήκης](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span><span class="sxs-lookup"><span data-stu-id="cfcd8-113">To make sure that your changes are crawled, you can specifically [request a re-indexing of the list or library](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span></span> 

<span data-ttu-id="cfcd8-114">Για μια πλήρη επισκόπηση του σχήματος αναζήτησης, ανατρέξτε στην ενότητα [Εισαγωγή σχήματος αναζήτησης](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span><span class="sxs-lookup"><span data-stu-id="cfcd8-114">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 


