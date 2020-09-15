---
title: το ίδιο με το όνομα αρχείου είναι καλύτερο
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 113d01e0fc92cc9845e585919ab05f386d6892bb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664134"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="c3a1c-102">"Η απαιτούμενη κεφαλίδα αλχημεία H1, H2's δεν λειτουργεί".</span><span class="sxs-lookup"><span data-stu-id="c3a1c-102">"Required Alchemy Header H1, H2's dont work."</span></span>
<span data-ttu-id="c3a1c-103">Βέλτιστες πρακτικές και οδηγίες για τη σύνταξη της αλχημείας:</span><span class="sxs-lookup"><span data-stu-id="c3a1c-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="c3a1c-104">Μην **κάνετε ένθεση ιδεών αλχημείας σε φακέλους**-αυτό θα διακόψει τη δομή της διεύθυνσης URL.</span><span class="sxs-lookup"><span data-stu-id="c3a1c-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="c3a1c-105">Ψάχνουμε να διορθώσουμε αυτό το θέμα.</span><span class="sxs-lookup"><span data-stu-id="c3a1c-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="c3a1c-106">Τα αρχεία στο φάκελο **AlchemyInsights** πρέπει να έχουν πεζά ονόματα αρχείων με ενωτικά για τα διαστήματα ex.</span><span class="sxs-lookup"><span data-stu-id="c3a1c-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="c3a1c-107">οδηγίες-ενεργοποίηση-εκκρεμείς ***δραστηριότητες-αναμονή***.</span><span class="sxs-lookup"><span data-stu-id="c3a1c-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="c3a1c-108">Συμπεριλάβετε το αναγνωριστικό κανόνα ή το αναγνωριστικό κάδου από την [πύλη συνεργάτη αλχημείας](https://alchemyportal.azurewebsites.net) στο πεδίο MS. Custom.</span><span class="sxs-lookup"><span data-stu-id="c3a1c-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="c3a1c-109">πρώην.</span><span class="sxs-lookup"><span data-stu-id="c3a1c-109">ex.</span></span> <span data-ttu-id="c3a1c-110">***MS. Custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="c3a1c-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="c3a1c-111">Χρησιμοποιήστε τα υπόλοιπα μετα-δεδομένα στο επάνω μέρος αυτού του αρχείου ως προτύπου.</span><span class="sxs-lookup"><span data-stu-id="c3a1c-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="c3a1c-112">Στην [πύλη συνεργατών του Alchemy](https://alchemyportal.azurewebsites.net), μετακινηθείτε προς τα κάτω στην ενότητα **Τίτλος διορατικότητας πελάτη:** και χρησιμοποιήστε το ως σημείο εκκίνησης για τον τίτλο H1 για τη διορατικότητα.</span><span class="sxs-lookup"><span data-stu-id="c3a1c-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="c3a1c-113">Οι ιδέες αλχημεία πρέπει να έχουν μόνο ένα H1 στο επάνω μέρος ή θα διασπάσουν την παραγωγή.</span><span class="sxs-lookup"><span data-stu-id="c3a1c-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="c3a1c-114">Το H2s δεν αποδίδει, επομένως, χρησιμοποιήστε **έντονη γραφή** ή άλλες συμβάσεις για να υποδηλώσει ξεχωριστές ενότητες.</span><span class="sxs-lookup"><span data-stu-id="c3a1c-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="c3a1c-115">Στη συνέχεια, συμπληρώστε το σώμα κειμένου χρησιμοποιώντας το πρόχειρο υλικό στην ενότητα "στατιστικά στοιχεία πελατών" της σελίδας "κανόνας αλχημείας"</span><span class="sxs-lookup"><span data-stu-id="c3a1c-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="c3a1c-116">Οι λίστες με κουκκίδες είναι λεπτές</span><span class="sxs-lookup"><span data-stu-id="c3a1c-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="c3a1c-117">Λίστες με αρίθμηση επίσης</span><span class="sxs-lookup"><span data-stu-id="c3a1c-117">Numbered lists too</span></span>
    1. <span data-ttu-id="c3a1c-118">Η **έντονη** γραφή και η *πλάγια γραφή* είναι a-OK</span><span class="sxs-lookup"><span data-stu-id="c3a1c-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="c3a1c-119">Οι συνδέσεις πρέπει να είναι πάντα είτε **"συνδέσεις στο Web"/External** είτε **βαθιές συνδέσεις με στοιχεία του περιβάλλοντος εργασίας χρήστη**, όχι εσωτερικές συνδέσεις.</span><span class="sxs-lookup"><span data-stu-id="c3a1c-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="c3a1c-120">Οι εικόνες δεν υποστηρίζονται επίσημα αυτήν τη στιγμή, αλλά είναι στον χάρτη πορείας.</span><span class="sxs-lookup"><span data-stu-id="c3a1c-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="c3a1c-121">Και αυτό είναι πραγματικά ήδη λίγο πολύ μεγάλο.</span><span class="sxs-lookup"><span data-stu-id="c3a1c-121">And this is really already a bit too long.</span></span> <span data-ttu-id="c3a1c-122">Η βέλτιστη πρακτική είναι περίπου 400 χαρακτήρες---------------------------------</span><span class="sxs-lookup"><span data-stu-id="c3a1c-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="c3a1c-123">Όταν το περιεχόμενό σας είναι έτοιμο, τραβήξτε το στο ζωντανό υποκατάστημα.</span><span class="sxs-lookup"><span data-stu-id="c3a1c-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="c3a1c-124">Στη συνέχεια, μεταβείτε στην [πύλη συνεργατών του Alchemy](https://alchemyportal.azurewebsites.net) και εισαγάγετε το όνομα αρχείου στο πεδίο διεύθυνση URL.</span><span class="sxs-lookup"><span data-stu-id="c3a1c-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 