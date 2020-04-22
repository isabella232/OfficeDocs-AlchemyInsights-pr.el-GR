---
title: ίδιο με το όνομα αρχείου είναι καλύτερο
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: e2dcca1295e37007593b34c2d818ad1d1133e4a1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676533"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="0c6c7-102">Απαιτείται Αλχημεία Header H1, H2 δεν λειτουργούν.</span><span class="sxs-lookup"><span data-stu-id="0c6c7-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="0c6c7-103">Βέλτιστες πρακτικές και κατευθυντήριες γραμμές για την αλχημεία συγγραφής:</span><span class="sxs-lookup"><span data-stu-id="0c6c7-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="0c6c7-104">**Μην φωλιάσετε αλχημεία Insights σε φακέλους**- αυτό θα σπάσει τη δομή url.</span><span class="sxs-lookup"><span data-stu-id="0c6c7-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="0c6c7-105">Ψάχνουμε να το διορθώσουμε.</span><span class="sxs-lookup"><span data-stu-id="0c6c7-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="0c6c7-106">Τα αρχεία στο φάκελο **AlchemyInsights** θα πρέπει να έχουν πεζά ονόματα αρχείων με ενωτικά για κενά ex.</span><span class="sxs-lookup"><span data-stu-id="0c6c7-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="0c6c7-107">***διαδικασία ενεργοποίησης-επίλυσης διαφορών***.</span><span class="sxs-lookup"><span data-stu-id="0c6c7-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="0c6c7-108">Συμπεριλάβετε το αναγνωριστικό κανόνα ή το αναγνωριστικό κάδου από την [πύλη "Συνεργάτης αλχημείας"](https://alchemyportal.azurewebsites.net) στο πεδίο ms.custom.</span><span class="sxs-lookup"><span data-stu-id="0c6c7-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="0c6c7-109">Ex.</span><span class="sxs-lookup"><span data-stu-id="0c6c7-109">ex.</span></span> <span data-ttu-id="0c6c7-110">***ms.custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="0c6c7-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="0c6c7-111">Χρησιμοποιήστε τα υπόλοιπα μετα-δεδομένα στο επάνω μέρος αυτού του αρχείου ως πρότυπο.</span><span class="sxs-lookup"><span data-stu-id="0c6c7-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="0c6c7-112">Στην [πύλη "Συνεργάτης αλχημείας",](https://alchemyportal.azurewebsites.net)μεταβείτε στην ενότητα **Τίτλος πληροφοριών πελατών:** και χρησιμοποιήστε το ως σημείο εκκίνησης για τον τίτλο H1 για τη διορατικότητα.</span><span class="sxs-lookup"><span data-stu-id="0c6c7-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="0c6c7-113">Αλχημεία Insights πρεπει να έχουν μόνο ένα H1 στην κορυφή ή θα σπάσει στην παραγωγή.</span><span class="sxs-lookup"><span data-stu-id="0c6c7-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="0c6c7-114">H2s δεν καθιστούν είτε έτσι χρησιμοποιούν **έντονη ή** άλλες συμβάσεις για να δηλώσει ξεχωριστές ενότητες.</span><span class="sxs-lookup"><span data-stu-id="0c6c7-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="0c6c7-115">Στη συνέχεια, συμπληρώστε το σώμα κειμένου χρησιμοποιώντας το πρόχειρο υλικό στην ενότητα Πληροφορίες πελατών της σελίδας "Κανόνας αλχημείας"</span><span class="sxs-lookup"><span data-stu-id="0c6c7-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="0c6c7-116">Οι λίστες με κουκκίδες είναι μια χαρά</span><span class="sxs-lookup"><span data-stu-id="0c6c7-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="0c6c7-117">Αριθμημένες λίστες επίσης</span><span class="sxs-lookup"><span data-stu-id="0c6c7-117">Numbered lists too</span></span>
    1. <span data-ttu-id="0c6c7-118">**Έντονη** και *πλάγια γραφή* είναι a-ok</span><span class="sxs-lookup"><span data-stu-id="0c6c7-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="0c6c7-119">Σύνδεσμοι θα πρέπει πάντα να είναι είτε **"συνδέσεις με web"/ εξωτερικές** ή **βαθιές συνδέσεις με στοιχεία ui,** δεν εσωτερικούς συνδέσμους.</span><span class="sxs-lookup"><span data-stu-id="0c6c7-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="0c6c7-120">Οι εικόνες δεν υποστηρίζονται επίσημα αυτή τη στιγμή, αλλά είναι στον οδικό χάρτη.</span><span class="sxs-lookup"><span data-stu-id="0c6c7-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="0c6c7-121">Και αυτό είναι πραγματικά ήδη λίγο πολύ μεγάλο.</span><span class="sxs-lookup"><span data-stu-id="0c6c7-121">And this is really already a bit too long.</span></span> <span data-ttu-id="0c6c7-122">Βέλτιστη πρακτική είναι περίπου 400 χαρακτήρες ---------------------------------</span><span class="sxs-lookup"><span data-stu-id="0c6c7-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="0c6c7-123">Μόλις το περιεχόμενό σας είναι έτοιμο, τραβήξτε το στο live υποκατάστημα.</span><span class="sxs-lookup"><span data-stu-id="0c6c7-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="0c6c7-124">Στη συνέχεια, μεταβείτε στην [πύλη "Συνεργάτης αλχημείας"](https://alchemyportal.azurewebsites.net) και εισαγάγετε το όνομα αρχείου στο πεδίο url.</span><span class="sxs-lookup"><span data-stu-id="0c6c7-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 