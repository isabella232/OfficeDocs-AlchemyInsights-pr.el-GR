---
title: Διαχείριση σχήμα αναζήτησης στο SharePoint Online
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 704fb3b682d23220d61192e383d7d80f59f27933
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36502807"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="bea29-102">Διαχείριση σχήμα αναζήτησης στο SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="bea29-102">Manage search schema in SharePoint Online</span></span>

<span data-ttu-id="bea29-103">Το σχήμα αναζήτησης ελέγχει τι να αναζητήσετε τους χρήστες, τον τρόπο στους χρήστες να τα αναζητάτε και πώς μπορείτε να παρουσιάσετε τα αποτελέσματα σε σας τοποθεσίες Web αναζήτησης.</span><span class="sxs-lookup"><span data-stu-id="bea29-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="bea29-104">Ανατρέξτε στην ενότητα [Διαχείριση σχήμα αναζήτησης στο SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) για να μάθετε πώς να:</span><span class="sxs-lookup"><span data-stu-id="bea29-104">See [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) to learn how to:</span></span> 
- <span data-ttu-id="bea29-105">Για να αλλάξετε το σχήμα αναζήτησης.</span><span class="sxs-lookup"><span data-stu-id="bea29-105">Change the search schema.</span></span>
- <span data-ttu-id="bea29-106">Δημιουργία διαχειριζόμενων ιδιοτήτων.</span><span class="sxs-lookup"><span data-stu-id="bea29-106">Create managed properties.</span></span>
- <span data-ttu-id="bea29-107">Χάρτης ανίχνευσης χάρτη ανιχνευόμενες ιδιότητες σε διαχειριζόμενες ιδιότητες.</span><span class="sxs-lookup"><span data-stu-id="bea29-107">Map crawled map crawled properties to managed properties.</span></span>

<span data-ttu-id="bea29-108">Σημειώστε τα εξής σε σχέση με τη Διαχείριση το σχήμα αναζήτησης:</span><span class="sxs-lookup"><span data-stu-id="bea29-108">Note the following in regards to managing your Search Schema:</span></span>

- <span data-ttu-id="bea29-109">Εάν λάβετε ένα προειδοποιητικό μήνυμα που θα αναφέρει **την παύση της εφαρμογής** όταν πραγματοποιείτε μια αλλαγή σχήματος, αυτό είναι μόνο προσωρινές καθώς δεν υπάρχει υπηρεσία συντήρησης που προκύπτουν.</span><span class="sxs-lookup"><span data-stu-id="bea29-109">If you receive a warning stating **the application is paused** when making a schema change, this is only temporary as there is service maintenance occurring.</span></span> 

    <span data-ttu-id="bea29-110">Εάν έχουν περάσει περισσότερες από 24 ώρες και εξακολουθείτε να αντιμετωπίζετε αυτό το προειδοποιητικό μήνυμα, συνδεθείτε μια υπόθεση υποστήριξης.</span><span class="sxs-lookup"><span data-stu-id="bea29-110">If more than 24 hours have passed and you still experience the warning, please log a support case.</span></span>
- <span data-ttu-id="bea29-111">Όταν αλλάζετε τις διαχειριζόμενες ιδιότητες ή προσθέσετε νέες, οι αλλαγές τεθούν σε ισχύ μόνο μετά το περιεχόμενο που έχει εκ νέου ανίχνευσης.</span><span class="sxs-lookup"><span data-stu-id="bea29-111">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="bea29-112">Με την ηλεκτρονική του SharePoint ανίχνευση συμβαίνει αυτόματα με βάση το χρονοδιάγραμμα ορίζεται ανίχνευσης.</span><span class="sxs-lookup"><span data-stu-id="bea29-112">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>
- <span data-ttu-id="bea29-113">Για να βεβαιωθείτε ότι είναι ανίχνευση για τις αλλαγές σας, μπορείτε να κάνετε συγκεκριμένα [αίτηση εκ νέου ευρετηρίου από τη λίστα ή τη βιβλιοθήκη](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span><span class="sxs-lookup"><span data-stu-id="bea29-113">To make sure that your changes are crawled, you can specifically [request a re-indexing of the list or library](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span></span> 

<span data-ttu-id="bea29-114">Για μια πλήρη επισκόπηση του σχήματος αναζήτησης, ανατρέξτε στην ενότητα [Εισαγωγή σχήματος αναζήτησης](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span><span class="sxs-lookup"><span data-stu-id="bea29-114">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 


