---
title: 'ίδιο με το όνομα αρχείου είναι καλύτερη [ΚΑΝΌΝΑ #-περιγραφή]'
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 278a26f4b986a85e33442baef690d3bb44462ace
ms.sourcegitcommit: 32355b76d45b730a069575efeec708149d4aeaa3
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 02/01/2019
ms.locfileid: "29697130"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="34b94-102">Απαιτείται "Alchemy" Επικεφαλίδα H1, H2 του δεν λειτουργούν.</span><span class="sxs-lookup"><span data-stu-id="34b94-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="34b94-103">Βέλτιστες πρακτικές και οδηγίες για τη σύνταξη "Alchemy":</span><span class="sxs-lookup"><span data-stu-id="34b94-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="34b94-p101">**Η ένθεση δεν είναι "Alchemy" ιδέες σε φακέλους**- αυτό θα διακόψει τη δομή της διεύθυνσης url. Κοιτάζουμε στον καθορισμό αυτό.</span><span class="sxs-lookup"><span data-stu-id="34b94-p101">**Do not nest Alchemy Insights in folders**- this will break the url structure. We're looking into fixing this.</span></span>
1. <span data-ttu-id="34b94-106">Αρχεία στο φάκελο **AlchemyInsights** πρέπει να έχουν Αναγνωριστικό κανόνα και το όνομα του κανόνα από την [πύλη συνεργάτη "Alchemy"](https://alchemyportal.azurewebsites.net) στο όνομα αρχείου.</span><span class="sxs-lookup"><span data-stu-id="34b94-106">Files in the **AlchemyInsights** folder should have Rule ID and Rule Name from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the filename.</span></span>
    1. <span data-ttu-id="34b94-p102">π.χ. ***976-How-to-enable-litigation-hold***</span><span class="sxs-lookup"><span data-stu-id="34b94-p102">ex. ***976-How-to-enable-litigation-hold***</span></span>
1. <span data-ttu-id="34b94-p103">Χρησιμοποιήστε τα μετα-δεδομένα στο επάνω μέρος αυτού του αρχείου ως προτύπου. Κανένα άλλο απαιτείται.</span><span class="sxs-lookup"><span data-stu-id="34b94-p103">Use the metadata at the top of this file as your template. Nothing else is required.</span></span>
1. <span data-ttu-id="34b94-111">Στην [πύλη συνεργάτη "Alchemy"](https://alchemyportal.azurewebsites.net), μετακινηθείτε προς τα κάτω, στην ενότητα **πελάτη πληροφορίες τίτλου:** και χρήση που παραπέμπουν ως μια έναρξης για τον τίτλο H1 σας για τις πληροφορίες.</span><span class="sxs-lookup"><span data-stu-id="34b94-111">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="34b94-p104">"Alchemy" ιδέες πρέπει να έχει μόνο μια μεμονωμένη H1 στο επάνω είτε θα διακόψετε παραγωγής. H2s δεν αποδώσει είτε έτσι χρήση **με έντονη γραφή** ή άλλες συμβάσεις για να προσδιορίσετε τις ξεχωριστές ενότητες.</span><span class="sxs-lookup"><span data-stu-id="34b94-p104">Alchemy Insights MUST have only a single H1 at the top or they will break in production. H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="34b94-114">Στη συνέχεια, συμπληρώστε το σώμα κειμένου χρησιμοποιώντας το υλικό σχέδιο στην ενότητα ιδέες πελατών της σελίδας κανόνα "Alchemy"</span><span class="sxs-lookup"><span data-stu-id="34b94-114">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="34b94-115">Λίστες με κουκκίδες είναι εξαιρετική</span><span class="sxs-lookup"><span data-stu-id="34b94-115">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="34b94-116">Λίστες με αρίθμηση πολύ</span><span class="sxs-lookup"><span data-stu-id="34b94-116">Numbered lists too</span></span>
    1. <span data-ttu-id="34b94-117">**Έντονη γραφή** και *πλάγια γραφή* είναι a-ok</span><span class="sxs-lookup"><span data-stu-id="34b94-117">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="34b94-118">Συνδέσεις πρέπει να είναι πάντοτε είτε **"συνδέσεις web" / εξωτερική** ή **deep-συνδέσεις σε στοιχεία περιβάλλοντος εργασίας Χρήστη**, όχι εσωτερικές συνδέσεις.</span><span class="sxs-lookup"><span data-stu-id="34b94-118">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>

<span data-ttu-id="34b94-p105">Και αυτό είναι πραγματικά ήδη λίγο πολύ μεγάλη. Η καλύτερη πρακτική είναι περίπου 400 χαρακτήρες---</span><span class="sxs-lookup"><span data-stu-id="34b94-p105">And this is really already a bit too long. Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="34b94-p106">Όταν το περιεχόμενο είναι έτοιμη, ελκυστική για το ζωντανό κλαδί. Στη συνέχεια, μεταβείτε στην [πύλη συνεργάτη "Alchemy"](https://alchemyportal.azurewebsites.net) και εισαγάγετε το όνομα του αρχείου στο πεδίο url. Βεβαιωθείτε ότι οι πληροφορίες για την αναθεώρηση και τη δημοσίευση αναφέρει ότι "Ναι" και, στη συνέχεια, κάντε κλικ στο κουμπί κανόνας ενημέρωσης. **(Αυτό θα φαίνεται prettier στη νέα έκδοση της πύλης - αποδέσμευση σύντομα.)** 
 ![πεδίο url](media/for-content-team.PNG)</span><span class="sxs-lookup"><span data-stu-id="34b94-p106">Once your content is ready, pull it to the live branch. Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field. Make sure Insight reviewed and published says "yes" and then click Update Rule. **(This will look prettier in the new version of the portal - releasing soon.)**
![url field](media/for-content-team.PNG)</span></span>

