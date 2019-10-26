---
title: ίδιο με το όνομα αρχείου είναι καλύτερο
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
ms.openlocfilehash: 31a578800468e9f3a69fff4f6e2e1945943c779c
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 10/25/2019
ms.locfileid: "35800045"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="b786a-102">Απαιτούμενη αλχημεία κεφαλίδα Η1, H2's δεν λειτουργούν.</span><span class="sxs-lookup"><span data-stu-id="b786a-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="b786a-103">Βέλτιστες πρακτικές και οδηγίες για τη σύνταξη αλχημείας:</span><span class="sxs-lookup"><span data-stu-id="b786a-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="b786a-104">Μην **φωλιάζουν αλχημεία στατιστικά σε φακέλους**-αυτό θα σπάσει τη δομή της διεύθυνσης URL.</span><span class="sxs-lookup"><span data-stu-id="b786a-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="b786a-105">Ψάχνουμε να το διορθώσουμε αυτό.</span><span class="sxs-lookup"><span data-stu-id="b786a-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="b786a-106">Τα αρχεία στο φάκελο **AlchemyInsights** πρέπει να έχουν πεζά ονόματα αρχείων με παύλες για διαστήματα ex.</span><span class="sxs-lookup"><span data-stu-id="b786a-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="b786a-107">***Πώς να ενεργοποιήσετε-επίλυση διαφορών-αναμονή***.</span><span class="sxs-lookup"><span data-stu-id="b786a-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="b786a-108">Συμπεριλάβετε το αναγνωριστικό κανόνα ή το αναγνωριστικό κάδου από την [πύλη συνεργάτη αλχημεία](https://alchemyportal.azurewebsites.net) στο πεδίο MS. Custom.</span><span class="sxs-lookup"><span data-stu-id="b786a-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="b786a-109">Ex.</span><span class="sxs-lookup"><span data-stu-id="b786a-109">ex.</span></span> <span data-ttu-id="b786a-110">***MS. έθιμο: 100021***</span><span class="sxs-lookup"><span data-stu-id="b786a-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="b786a-111">Χρησιμοποιήστε τα υπόλοιπα μεταδεδομένα στο επάνω μέρος αυτού του αρχείου ως πρότυπο.</span><span class="sxs-lookup"><span data-stu-id="b786a-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="b786a-112">Στην [πύλη των συνεργατών αλχημείας](https://alchemyportal.azurewebsites.net), μετακινηθείτε προς τα κάτω στην ενότητα **Τίτλος γνώσης πελάτη:** και χρησιμοποιήστε το ως σημείο εκκίνησης για τον τίτλο σας Η1 για την διορατικότητα.</span><span class="sxs-lookup"><span data-stu-id="b786a-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="b786a-113">Οι αλχημείες πρέπει να έχουν μόνο μία Η1 στην κορυφή ή θα σπάσουν στην παραγωγή.</span><span class="sxs-lookup"><span data-stu-id="b786a-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="b786a-114">Το H2s δεν αποδίδει ούτε τη χρήση **έντονης γραφής** ή άλλων συμβάσεων που υποδεικνύουν ξεχωριστές ενότητες.</span><span class="sxs-lookup"><span data-stu-id="b786a-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="b786a-115">Στη συνέχεια, συμπληρώστε το σώμα κειμένου χρησιμοποιώντας το σχέδιο υλικού στην ενότητα Πληροφορίες πελάτη της σελίδας "κανόνας αλχημείας"</span><span class="sxs-lookup"><span data-stu-id="b786a-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="b786a-116">Οι λίστες με κουκκίδες είναι εντάξει</span><span class="sxs-lookup"><span data-stu-id="b786a-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="b786a-117">Και οι αριθμημένες λίστες</span><span class="sxs-lookup"><span data-stu-id="b786a-117">Numbered lists too</span></span>
    1. <span data-ttu-id="b786a-118">Η **έντονη** και η *πλάγια γραφή* είναι a-OK</span><span class="sxs-lookup"><span data-stu-id="b786a-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="b786a-119">Οι συνδέσεις πρέπει πάντα να είναι είτε **"συνδέσεις στο Web"/εξωτερικές** ή **Deep-ΣΥΝΔΈΣΕΙς σε στοιχεία UI**, όχι εσωτερικές συνδέσεις.</span><span class="sxs-lookup"><span data-stu-id="b786a-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="b786a-120">Οι εικόνες δεν υποστηρίζονται επισήμως αυτή τη στιγμή, αλλά είναι στον οδικό χάρτη.</span><span class="sxs-lookup"><span data-stu-id="b786a-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="b786a-121">Και αυτό είναι πολύ μεγάλο.</span><span class="sxs-lookup"><span data-stu-id="b786a-121">And this is really already a bit too long.</span></span> <span data-ttu-id="b786a-122">Η βέλτιστη πρακτική είναι περίπου 400 χαρακτήρες---------------------------------</span><span class="sxs-lookup"><span data-stu-id="b786a-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="b786a-123">Μόλις το περιεχόμενό σας είναι έτοιμο, τραβήξτε το στο ζωντανό κλαδί.</span><span class="sxs-lookup"><span data-stu-id="b786a-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="b786a-124">Στη συνέχεια, μεταβείτε στην [πύλη συνεργάτη αλχημείας](https://alchemyportal.azurewebsites.net) και εισαγάγετε το όνομα αρχείου στο πεδίο URL.</span><span class="sxs-lookup"><span data-stu-id="b786a-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 