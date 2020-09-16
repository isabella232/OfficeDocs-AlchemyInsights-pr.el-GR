---
title: Διαχείριση σχήματος αναζήτησης στο SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: f2d8d3e07fe32d21af484e4c59e0f5ac6fe8081c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47770551"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="48b70-102">Διαχείριση σχήματος αναζήτησης στο SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="48b70-102">Manage search schema in SharePoint Online</span></span>

<span data-ttu-id="48b70-103">Το σχήμα αναζήτησης ελέγχει τι μπορούν να αναζητήσουν οι χρήστες, τον τρόπο με τον οποίο οι χρήστες μπορούν να το αναζητήσουν και τον τρόπο με τον οποίο μπορείτε να παρουσιάσετε τα αποτελέσματα στις τοποθεσίες Web αναζήτησης.</span><span class="sxs-lookup"><span data-stu-id="48b70-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="48b70-104">Ανατρέξτε στο θέμα [Διαχείριση του σχήματος αναζήτησης στο SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) για να μάθετε πώς μπορείτε να κάνετε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="48b70-104">See [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) to learn how to:</span></span> 
- <span data-ttu-id="48b70-105">Αλλάξτε το σχήμα αναζήτησης.</span><span class="sxs-lookup"><span data-stu-id="48b70-105">Change the search schema.</span></span>
- <span data-ttu-id="48b70-106">Δημιουργία διαχειριζόμενων ιδιοτήτων.</span><span class="sxs-lookup"><span data-stu-id="48b70-106">Create managed properties.</span></span>
- <span data-ttu-id="48b70-107">Αντιστοίχιση ανιχνευμένου χάρτη ανιχνευμένων ιδιοτήτων σε διαχειριζόμενες ιδιότητες.</span><span class="sxs-lookup"><span data-stu-id="48b70-107">Map crawled map crawled properties to managed properties.</span></span>

<span data-ttu-id="48b70-108">Λάβετε υπόψη σας τα εξής σχετικά με τη διαχείριση του σχήματος αναζήτησης:</span><span class="sxs-lookup"><span data-stu-id="48b70-108">Note the following in regards to managing your Search Schema:</span></span>

- <span data-ttu-id="48b70-109">Εάν λάβετε μια προειδοποίηση που αναφέρει ότι **η εφαρμογή έχει διακοπεί προσωρινά** κατά τη δημιουργία μιας αλλαγής σχήματος, αυτό είναι μόνο προσωρινό, καθώς εμφανίζεται η συντήρηση υπηρεσίας.</span><span class="sxs-lookup"><span data-stu-id="48b70-109">If you receive a warning stating **the application is paused** when making a schema change, this is only temporary as there is service maintenance occurring.</span></span> 

    <span data-ttu-id="48b70-110">Εάν έχουν περάσει περισσότερες από 24 ώρες και εξακολουθείτε να αντιμετωπίζετε την προειδοποίηση, καταγράψτε μια υπόθεση υποστήριξης.</span><span class="sxs-lookup"><span data-stu-id="48b70-110">If more than 24 hours have passed and you still experience the warning, please log a support case.</span></span>
- <span data-ttu-id="48b70-111">Όταν αλλάζετε τις διαχειριζόμενες ιδιότητες ή προσθέτετε νέες, οι αλλαγές εφαρμόζονται μόνο μετά την εκ νέου ανίχνευση του περιεχομένου.</span><span class="sxs-lookup"><span data-stu-id="48b70-111">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="48b70-112">Στο SharePoint Online, η ανίχνευση γίνεται αυτόματα με βάση το καθορισμένο χρονοδιάγραμμα ανίχνευσης.</span><span class="sxs-lookup"><span data-stu-id="48b70-112">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>
- <span data-ttu-id="48b70-113">Για να βεβαιωθείτε ότι οι αλλαγές σας ανιχνεύονται, μπορείτε να ζητήσετε συγκεκριμένα την [εκ νέου δημιουργία ευρετηρίου της λίστας ή της βιβλιοθήκης](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span><span class="sxs-lookup"><span data-stu-id="48b70-113">To make sure that your changes are crawled, you can specifically [request a re-indexing of the list or library](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span></span> 

<span data-ttu-id="48b70-114">Για μια ολοκληρωμένη επισκόπηση του σχήματος αναζήτησης, ανατρέξτε στο θέμα [Εισαγωγή σχήματος αναζήτησης](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span><span class="sxs-lookup"><span data-stu-id="48b70-114">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 


