---
title: ίδιο με το όνομα αρχείου είναι καλύτερα
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: b77e514da36701808d46248e8f2a45137751a1c7
ms.sourcegitcommit: 5447031f9d0a320c49897b8adb5d29ac9437fbc5
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 07/18/2019
ms.locfileid: "35786413"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="280d0-102">Απαιτείται "Alchemy" Επικεφαλίδα H1, H2 του δεν λειτουργούν.</span><span class="sxs-lookup"><span data-stu-id="280d0-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="280d0-103">Βέλτιστες πρακτικές και οδηγίες για τη σύνταξη "Alchemy":</span><span class="sxs-lookup"><span data-stu-id="280d0-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="280d0-104">**Η ένθεση δεν είναι "Alchemy" ιδέες σε φακέλους**- αυτό θα διακόψει τη δομή της διεύθυνσης url.</span><span class="sxs-lookup"><span data-stu-id="280d0-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="280d0-105">Κοιτάζουμε στον καθορισμό αυτό.</span><span class="sxs-lookup"><span data-stu-id="280d0-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="280d0-106">Αρχεία στο φάκελο **AlchemyInsights** πρέπει να έχουν πεζούς ονόματα με παύλες, κενά ex.</span><span class="sxs-lookup"><span data-stu-id="280d0-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="280d0-107">***how-σε-Ενεργοποίηση-δίκη-αναμονή***.</span><span class="sxs-lookup"><span data-stu-id="280d0-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="280d0-108">Συμπεριλάβετε το Αναγνωριστικό του κανόνα ή Κάδου ID από την [πύλη συνεργάτη "Alchemy"](https://alchemyportal.azurewebsites.net) στο πεδίο ms.custom.</span><span class="sxs-lookup"><span data-stu-id="280d0-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="280d0-109">ex.</span><span class="sxs-lookup"><span data-stu-id="280d0-109">ex.</span></span> <span data-ttu-id="280d0-110">***MS.Custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="280d0-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="280d0-111">Χρησιμοποιήστε τα υπόλοιπα μετα-δεδομένα, στο επάνω μέρος αυτού του αρχείου ως προτύπου.</span><span class="sxs-lookup"><span data-stu-id="280d0-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="280d0-112">Στην [πύλη συνεργάτη "Alchemy"](https://alchemyportal.azurewebsites.net), μετακινηθείτε προς τα κάτω, στην ενότητα **πελάτη πληροφορίες τίτλου:** και χρήση που παραπέμπουν ως μια έναρξης για τον τίτλο H1 σας για τις πληροφορίες.</span><span class="sxs-lookup"><span data-stu-id="280d0-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="280d0-113">"Alchemy" ιδέες πρέπει να έχει μόνο μια μεμονωμένη H1 στο επάνω είτε θα διακόψετε παραγωγής.</span><span class="sxs-lookup"><span data-stu-id="280d0-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="280d0-114">H2s δεν αποδώσει είτε έτσι χρήση **με έντονη γραφή** ή άλλες συμβάσεις για να προσδιορίσετε τις ξεχωριστές ενότητες.</span><span class="sxs-lookup"><span data-stu-id="280d0-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="280d0-115">Στη συνέχεια, συμπληρώστε το σώμα κειμένου χρησιμοποιώντας το υλικό σχέδιο στην ενότητα ιδέες πελατών της σελίδας κανόνα "Alchemy"</span><span class="sxs-lookup"><span data-stu-id="280d0-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="280d0-116">Λίστες με κουκκίδες είναι εξαιρετική</span><span class="sxs-lookup"><span data-stu-id="280d0-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="280d0-117">Λίστες με αρίθμηση πολύ</span><span class="sxs-lookup"><span data-stu-id="280d0-117">Numbered lists too</span></span>
    1. <span data-ttu-id="280d0-118">**Έντονη γραφή** και *πλάγια γραφή* είναι a-ok</span><span class="sxs-lookup"><span data-stu-id="280d0-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="280d0-119">Συνδέσεις πρέπει να είναι πάντοτε είτε **"συνδέσεις web" / εξωτερική** ή **deep-συνδέσεις σε στοιχεία περιβάλλοντος εργασίας Χρήστη**, όχι εσωτερικές συνδέσεις.</span><span class="sxs-lookup"><span data-stu-id="280d0-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="280d0-120">Οι εικόνες δεν υποστηρίζονται επίσημα αυτήν τη στιγμή, αλλά είναι σχετικά με το χάρτη.</span><span class="sxs-lookup"><span data-stu-id="280d0-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="280d0-121">Και αυτό είναι πραγματικά ήδη λίγο πολύ μεγάλη.</span><span class="sxs-lookup"><span data-stu-id="280d0-121">And this is really already a bit too long.</span></span> <span data-ttu-id="280d0-122">Η καλύτερη πρακτική είναι περίπου 400 χαρακτήρες---</span><span class="sxs-lookup"><span data-stu-id="280d0-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="280d0-123">Όταν το περιεχόμενο είναι έτοιμη, ελκυστική για το ζωντανό κλαδί.</span><span class="sxs-lookup"><span data-stu-id="280d0-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="280d0-124">Στη συνέχεια, μεταβείτε στην [πύλη συνεργάτη "Alchemy"](https://alchemyportal.azurewebsites.net) και εισαγάγετε το όνομα του αρχείου στο πεδίο url.</span><span class="sxs-lookup"><span data-stu-id="280d0-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 


