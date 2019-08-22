---
title: Αναζήτηση στο SharePoint ηλεκτρονικά
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 3c3f6384172b2b4d59db6059618572db11059228
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507631"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a><span data-ttu-id="900fa-102">Ανίχνευση περιεχομένου και τη δημιουργία ευρετηρίου με την ηλεκτρονική του SharePoint</span><span class="sxs-lookup"><span data-stu-id="900fa-102">Content crawling and indexing in SharePoint Online</span></span>

<span data-ttu-id="900fa-103">Περιεχόμενο πρέπει να ανιχνεύεται και να προστεθεί στο ευρετήριο αναζήτησης για να βρείτε τι τους αναζητάτε στο SharePoint Online οι χρήστες.</span><span class="sxs-lookup"><span data-stu-id="900fa-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="900fa-104">Το περιεχόμενο ανιχνεύεται αυτόματα με βάση ένα χρονοδιάγραμμα προκαθορισμένες ανίχνευσης (δεν μπορεί να αλλάξει το χρονοδιάγραμμα ανίχνευσης).</span><span class="sxs-lookup"><span data-stu-id="900fa-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="900fa-105">Το πρόγραμμα ανίχνευσης παίρνει το περιεχόμενο που έχει αλλάξει από την τελευταία ανίχνευση και ενημερώνει το ευρετήριο.</span><span class="sxs-lookup"><span data-stu-id="900fa-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="900fa-106">Για να εξασφαλίσετε την ανίχνευση περιεχομένου και ενημερώνεται το ευρετήριο, σημειώστε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="900fa-106">To ensure content is crawled and the index is updated, note the following:</span></span>

- <span data-ttu-id="900fa-107">Βεβαιωθείτε ότι μπορείτε να βρείτε περιεχόμενο, [κάνοντας το περιεχόμενο της τοποθεσίας με δυνατότητα αναζήτησης](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="900fa-107">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="900fa-108">Όταν έχετε αλλάξει μια διαχειριζόμενη ιδιότητα ή όταν έχετε αλλάξει την αντιστοίχιση της ανίχνευσης και διαχείρισης ιδιότητες, η τοποθεσία πρέπει να είναι εκ νέου ανίχνευσης, πριν οι αλλαγές θα εμφανιστούν στο ευρετήριο αναζήτησης.</span><span class="sxs-lookup"><span data-stu-id="900fa-108">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

    <span data-ttu-id="900fa-109">Επειδή οι αλλαγές σας γίνονται στο σχήμα της αναζήτησης και να μην την τρέχουσα τοποθεσία, το πρόγραμμα ανίχνευσης θα αυτόματα ευρετήριο εκ νέου την τοποθεσία.</span><span class="sxs-lookup"><span data-stu-id="900fa-109">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

    <span data-ttu-id="900fa-110">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [με μη αυτόματο τρόπο αίτηση ανίχνευσης και εκ νέου δημιουργία ευρετηρίου για μια τοποθεσία, μια βιβλιοθήκη ή λίστα](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span><span class="sxs-lookup"><span data-stu-id="900fa-110">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span></span>

- <span data-ttu-id="900fa-111">Περιμένετε τουλάχιστον 24 ώρες μετά την αίτηση με μη αυτόματο τρόπο μια ανίχνευση και πλήρες ευρετήριο εκ νέου για να δείτε εάν ακόμα αντιμετωπίζετε ένα ζήτημα.</span><span class="sxs-lookup"><span data-stu-id="900fa-111">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

    <span data-ttu-id="900fa-112">Εάν έχουν περάσει περισσότερες από 24 ώρες, εφόσον είστε ο ιδρυτής της ανίχνευσης και πλήρη αναδιοργανώστε σε μορφή ευρετηρίου, συνδεθείτε μια υπόθεση υποστήριξης.</span><span class="sxs-lookup"><span data-stu-id="900fa-112">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="900fa-113">Σε πολλές περιπτώσεις, εργαζόμαστε ήδη σε μια λύση.</span><span class="sxs-lookup"><span data-stu-id="900fa-113">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="900fa-114">Παρακαλούμε να μας δώσετε τουλάχιστον 24 ώρες για να ολοκληρωθεί μια λύση.</span><span class="sxs-lookup"><span data-stu-id="900fa-114">Please give us at least 24 hours to complete a solution.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="900fa-115">Εάν μια τοποθεσία, έγγραφο (βιβλιοθήκη) ή μια λίστα διαγράφηκε και εξακολουθεί να εμφανίζει στα αποτελέσματα αναζήτησης, οι χρήστες θα πρέπει να λαμβάνουν πληροφορίες ένα **Σφάλμα 404 το αρχείο δεν βρέθηκε** κατά την προσπάθεια πρόσβασης σε αυτό.</span><span class="sxs-lookup"><span data-stu-id="900fa-115">If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="900fa-116">Αυτό το ζήτημα θα πρέπει να έχετε συνδεθεί ως μια υπόθεση υποστήριξης για περαιτέρω έρευνα.</span><span class="sxs-lookup"><span data-stu-id="900fa-116">This issue should be logged as a support case for further investigation.</span></span> 



