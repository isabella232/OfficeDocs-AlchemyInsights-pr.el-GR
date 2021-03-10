---
title: Να γίνει εντοπισμός τοποθεσίας
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9143"
- "9005291"
ms.openlocfilehash: bdf94220de45d92f63e56501ea4e35389224d25c
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693488"
---
# <a name="do-site-discovery"></a><span data-ttu-id="f209c-102">Να γίνει εντοπισμός τοποθεσίας</span><span class="sxs-lookup"><span data-stu-id="f209c-102">Do site discovery</span></span>

<span data-ttu-id="f209c-103">Εάν η εταιρεία σας εξακολουθεί να χρησιμοποιεί εφαρμογές Web παλαιού τύπου και σχεδιάζει να χρησιμοποιήσει τη λειτουργία Internet Explorer (την οποία χρησιμοποιούν οι περισσότεροι πελάτες), θα πρέπει να κάνετε ορισμένες πρόσθετες ανακαλύψεις τοποθεσίας.</span><span class="sxs-lookup"><span data-stu-id="f209c-103">If your organization still uses legacy web applications and plans to use Internet Explorer mode (which most customers do), then you should do some additional site discovery.</span></span>

<span data-ttu-id="f209c-104">**Έχετε ήδη αναπτύξει μια παλαιότερη έκδοση του Microsoft Edge**</span><span class="sxs-lookup"><span data-stu-id="f209c-104">**You've already deployed an older version of Microsoft Edge**</span></span>

<span data-ttu-id="f209c-105">Εάν έχετε ήδη ρυθμίσει τις παραμέτρους της λίστας εταιρικών τοποθεσιών ώστε να λειτουργεί για την προηγούμενη έκδοση του Microsoft Edge, ο εντοπισμός της τοποθεσίας σας έχει σχεδόν γίνει.</span><span class="sxs-lookup"><span data-stu-id="f209c-105">If you've already configured your Enterprise Site List to work for the legacy version of Microsoft Edge, then your site discovery is almost done.</span></span> <span data-ttu-id="f209c-106">Το μόνο πράγμα που ίσως χρειαστεί να κάνετε είναι να προσθέσετε ουδέτερες τοποθεσίες.</span><span class="sxs-lookup"><span data-stu-id="f209c-106">The one thing you might need to do is add neutral sites.</span></span>

<span data-ttu-id="f209c-107">Οι ουδέτερες τοποθεσίες είναι συνήθως τοποθεσίες που παρέχουν ενιαία σύνδεση (SSO).</span><span class="sxs-lookup"><span data-stu-id="f209c-107">Neutral sites are typically sites that provide single sign-on (SSO).</span></span> <span data-ttu-id="f209c-108">Εάν μεταβείτε σε μια ουδέτερη τοποθεσία από τον Microsoft Edge, τότε θέλετε να παραμείνετε στον Microsoft Edge για έλεγχο ταυτότητας.</span><span class="sxs-lookup"><span data-stu-id="f209c-108">If you go to a neutral site from Microsoft Edge, then you want to stay in Microsoft Edge to authenticate.</span></span> <span data-ttu-id="f209c-109">Εάν μεταβείτε σε μια ουδέτερη τοποθεσία σε λειτουργία Internet Explorer, τότε θέλετε να παραμείνετε σε λειτουργία Internet Explorer για τον έλεγχο ταυτότητας.</span><span class="sxs-lookup"><span data-stu-id="f209c-109">If you go to a neutral site in Internet Explorer mode, then you want to stay in Internet Explorer mode to authenticate.</span></span>

<span data-ttu-id="f209c-110">Προσδιορίστε τυχόν SSO ή άλλες ουδέτερες τοποθεσίες που χρησιμοποιείτε και προσθέστε τις στη λίστα εταιρικών τοποθεσιών.</span><span class="sxs-lookup"><span data-stu-id="f209c-110">Identify any SSO or other neutral sites that you use and add these to your Enterprise Site List.</span></span>

<span data-ttu-id="f209c-111">**Ο Internet Explorer είναι το προεπιλεγμένο πρόγραμμα περιήγησης**</span><span class="sxs-lookup"><span data-stu-id="f209c-111">**Internet Explorer is your default browser**</span></span>

<span data-ttu-id="f209c-112">Εάν χρησιμοποιείτε μόνο τον Internet Explorer τώρα, ενδέχεται να μην γνωρίζετε ποιες τοποθεσίες έχουν αναβαθμιστεί σε σύγχρονα πρότυπα Web και ποια εξακολουθούν να απαιτούν internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="f209c-112">If you're only using Internet Explorer now, you might not know which sites have upgraded to modern web standards and which still require Internet Explorer.</span></span> <span data-ttu-id="f209c-113">Θα πρέπει να βρείτε και να προσθέσετε αυτές τις τοποθεσίες στη λίστα εταιρικών τοποθεσιών, ώστε να μπορείτε να χρησιμοποιήσετε τη λειτουργία Internet Explorer μόνο για αυτές τις τοποθεσίες.</span><span class="sxs-lookup"><span data-stu-id="f209c-113">You'll want to find and add these sites to the Enterprise Site List so that you can use Internet Explorer mode only for those sites.</span></span>

> [!NOTE]
> <span data-ttu-id="f209c-114">[Ο εντοπισμός εταιρικής](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) τοποθεσίας ανακαλύπτει τοποθεσίες που ενδέχεται να χρειάζονται τη λειτουργία Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="f209c-114">[Enterprise Site Discovery](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) discovers sites that might need Internet Explorer mode.</span></span> <span data-ttu-id="f209c-115">Μπορεί να συλλέγει δεδομένα σε υπολογιστές που εκτελούν Windows Internet Explorer 8 internet Explorer 11 σε Windows 10, Windows 8.1 ή Windows 7.</span><span class="sxs-lookup"><span data-stu-id="f209c-115">It can collect data on computers running Windows Internet Explorer 8 through Internet Explorer 11 on Windows 10, Windows 8.1, or Windows 7.</span></span>

<span data-ttu-id="f209c-116">**Ανάλυση των δεδομένων**</span><span class="sxs-lookup"><span data-stu-id="f209c-116">**Analyze the data**</span></span>

<span data-ttu-id="f209c-117">Αφού συλλέξετε δεδομένα τοποθεσίας, συνιστάται η παρακάτω διαδικασία τεσσάρων βημάτων για την ανάλυση των δεδομένων:</span><span class="sxs-lookup"><span data-stu-id="f209c-117">After you've collected site data, we recommend the following four-step process to analyze the data:</span></span>
1. <span data-ttu-id="f209c-118">Ταξινομήστε τα δεδομένα κατά τομέα και, στη συνέχεια, κατά διεύθυνση URL.</span><span class="sxs-lookup"><span data-stu-id="f209c-118">Sort the data by domain, and then by URL.</span></span>
2. <span data-ttu-id="f209c-119">Καθορίστε τα όρια μιας εφαρμογής για να ρυθμίσετε τις παραμέτρους για τη λειτουργία Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="f209c-119">Define the boundaries of an app to configure for Internet Explorer mode.</span></span> <span data-ttu-id="f209c-120">Θέλετε να συμπεριλάβετε όλες τις τοποθεσίες και τα στοιχεία ελέγχου Web που ορίζουν την εφαρμογή, αλλά δεν θέλετε να συμπεριλάβετε επιπλέον τοποθεσίες και στοιχεία ελέγχου.</span><span class="sxs-lookup"><span data-stu-id="f209c-120">You want to include all the sites and web controls that define the app, but you don't want to include extra sites and controls.</span></span> <span data-ttu-id="f209c-121">Ορισμένες τοποθεσίες μπορεί να είναι τόσο απλές *https://contoso.com/app1* όσο ενώ άλλες μπορεί να απαιτούν τον ορισμό πολλών τοποθεσιών και σελίδων.</span><span class="sxs-lookup"><span data-stu-id="f209c-121">Some sites might be as simple as *https://contoso.com/app1* while others might require you to define multiple sites and pages.</span></span>
3. <span data-ttu-id="f209c-122">Δοκιμάστε την εφαρμογή για να βεβαιωθείτε ότι δεν λειτουργεί εγγενώς.</span><span class="sxs-lookup"><span data-stu-id="f209c-122">Test the app to verify that it doesn't work natively.</span></span> <span data-ttu-id="f209c-123">Πολλές τοποθεσίες θα προσφέρουν σύγχρονο περιεχόμενο όταν εντοπίζουν ένα σύγχρονο πρόγραμμα περιήγησης και προσφέρουν περιεχόμενο παλαιού τύπου μόνο όταν εντοπίζουν τον Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="f209c-123">Many sites will offer modern content when they detect a modern browser and only offer legacy content when they detect Internet Explorer.</span></span>
4. <span data-ttu-id="f209c-124">Προσθέστε την εφαρμογή στη λίστα εταιρικών τοποθεσιών, εάν αποτύχει ο έλεγχος.</span><span class="sxs-lookup"><span data-stu-id="f209c-124">Add the app to your Enterprise Site List if it fails testing.</span></span>

> [!NOTE]
> <span data-ttu-id="f209c-125">Ως βέλτιστη πρακτική, ομαδοποιήσετε όλες τις τοποθεσίες που συνθέτουν μια εφαρμογή.</span><span class="sxs-lookup"><span data-stu-id="f209c-125">As a best practice, group all of the sites that comprise an app.</span></span> <span data-ttu-id="f209c-126">Με αυτόν τον τρόπο, όταν κάνετε αναβάθμιση μιας εφαρμογής, είναι πιο εύκολο να καταργήσετε ολόκληρη την τοποθεσία από τη λειτουργία Internet Explorer και να ξεκινήσετε να χρησιμοποιείτε ένα σύγχρονο πρόγραμμα περιήγησης για αυτή την εφαρμογή.</span><span class="sxs-lookup"><span data-stu-id="f209c-126">This way, when you upgrade an app, it's easier to remove the entire site from Internet Explorer mode and start using a modern browser for that app.</span></span>

<span data-ttu-id="f209c-127">Όταν τελειώσετε με τον εντοπισμό τοποθεσίας και αναλύσετε τα δεδομένα, είστε έτοιμοι να αρχίσετε να κοιτάτε τη στρατηγική καναλιού.</span><span class="sxs-lookup"><span data-stu-id="f209c-127">Once you're done with site discovery and you've analyzed the data, you're ready to start looking at your channel strategy.</span></span>

