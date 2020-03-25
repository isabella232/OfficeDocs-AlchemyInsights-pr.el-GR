---
title: Ζητήματα κατά τη μετεγκατάσταση δεδομένων στο SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "1885"
ms.openlocfilehash: b53a98480bab48497274c7358f7e606caa477f5a
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931694"
---
# <a name="issues-while-migrating-data-to-sharepoint-online"></a><span data-ttu-id="3a158-102">Ζητήματα κατά τη μετεγκατάσταση δεδομένων στο SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="3a158-102">Issues while migrating data to SharePoint Online</span></span>

<span data-ttu-id="3a158-103">**Σημαντικό:** Πολλοί πελάτες του SharePoint Online και του OneDrive εκτελούν κρίσιμες για την επιχείρηση εφαρμογές σε θέματα που εκτελούνται στο παρασκήνιο.</span><span class="sxs-lookup"><span data-stu-id="3a158-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="3a158-104">Σε αυτές περιλαμβάνονται η μετεγκατάσταση περιεχομένου, η Αποτροπή απώλειας δεδομένων (DLP) και οι λύσεις δημιουργίας αντιγράφων ασφαλείας.</span><span class="sxs-lookup"><span data-stu-id="3a158-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="3a158-105">Κατά τη διάρκεια αυτών των πρωτοφανών χρόνων, λαμβάνουμε μέτρα για να διασφαλίσουμε ότι οι υπηρεσίες Του SharePoint Online και του OneDrive παραμένουν ιδιαίτερα διαθέσιμες και αξιόπιστες για τους χρήστες σας που εξαρτώνται από την υπηρεσία περισσότερο από ποτέ σε σενάρια απομακρυσμένης εργασίας.</span><span class="sxs-lookup"><span data-stu-id="3a158-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="3a158-106">Για την υποστήριξη αυτού του στόχου, έχουμε εφαρμόσει αυστηρότερα όρια επιτάχυνσης στις εφαρμογές παρασκηνίου (μετανάστευση, DLP και λύσεις δημιουργίας αντιγράφων ασφαλείας) κατά τις καθημερινές ώρες της ημέρας.</span><span class="sxs-lookup"><span data-stu-id="3a158-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="3a158-107">Θα πρέπει να περιμένετε ότι αυτές οι εφαρμογές θα επιτύχουν πολύ περιορισμένη ρυθμοφορεία κατά τη διάρκεια αυτών των χρόνων.</span><span class="sxs-lookup"><span data-stu-id="3a158-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="3a158-108">Ωστόσο, κατά τις βραδινές ώρες και τις ώρες του Σαββατοκύριακου για την περιοχή, η υπηρεσία θα είναι έτοιμη να επεξεργαστεί έναν σημαντικά υψηλότερο όγκο αιτημάτων από εφαρμογές παρασκηνίου.</span><span class="sxs-lookup"><span data-stu-id="3a158-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="3a158-109">**Μετεγκατάσταση δεδομένων άνω των 100 TB**</span><span class="sxs-lookup"><span data-stu-id="3a158-109">**Migrating over 100TB of data**</span></span>

<span data-ttu-id="3a158-110">Φαίνεται ότι μετεγκαθιστάτε πάνω από 100 TB δεδομένων στο SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="3a158-110">It appears you are migrating over 100TB of data to SharePoint Online.</span></span> <span data-ttu-id="3a158-111">Ακολουθήστε τα παρακάτω βήματα, ώστε να σας βοηθήσουμε το συντομότερο δυνατό.</span><span class="sxs-lookup"><span data-stu-id="3a158-111">Please follow the steps below so we may assist you as soon as possible.</span></span> 

1. <span data-ttu-id="3a158-112">Επιλέξτε **Νέα αίτηση τ/υ**και, στη συνέχεια, **Νέα αίτηση τ/υ**.</span><span class="sxs-lookup"><span data-stu-id="3a158-112">Select **New Service Request**, and then **New Service Request**.</span></span> 
2. <span data-ttu-id="3a158-113">Αφήστε τον τίτλο και την περιγραφή ως **μετεγκατάσταση του SharePoint πάνω από 100TB**.</span><span class="sxs-lookup"><span data-stu-id="3a158-113">Leave the title and description as **SharePoint migration over 100TB**.</span></span>
3. <span data-ttu-id="3a158-114">Μόλις υποβληθεί το εισιτήριο, παρακαλείστε να το ενημερώσετε με τις ακόλουθες πληροφορίες:</span><span class="sxs-lookup"><span data-stu-id="3a158-114">Once the ticket has been submitted, please update it with the following information:</span></span> 

    - <span data-ttu-id="3a158-115">Εκτιμώμενο μέγεθος της μετεγκατάστασης.</span><span class="sxs-lookup"><span data-stu-id="3a158-115">Estimated size of your migration.</span></span>
    - <span data-ttu-id="3a158-116">Μια εκτίμηση για το πότε θέλετε να ξεκινήσετε και να ολοκληρώσετε τη μετεγκατάσταση.</span><span class="sxs-lookup"><span data-stu-id="3a158-116">An estimate of when you would like to start and complete your migration.</span></span>
    - <span data-ttu-id="3a158-117">Περιγράψτε από πού μετεγκαθιστάτε το περιεχόμενό σας, όπως sharePoint Server, Box, GDrive, Κοινόχρηστα στοιχεία αρχείων κ.λπ..</span><span class="sxs-lookup"><span data-stu-id="3a158-117">Describe where you are migrating your content from, such as SharePoint Server, Box, GDrive, File shares, etc..</span></span>


  

