---
title: Θέματα που σχετίζονται με vpn
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1545"
- "9000076"
ms.openlocfilehash: 134d78f30216dfd268c5999a5032b7d7ad1d7dd8
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 07/28/2020
ms.locfileid: "46554968"
---
# <a name="vpn-related-issues"></a><span data-ttu-id="fcf4d-102">Θέματα που σχετίζονται με vpn</span><span class="sxs-lookup"><span data-stu-id="fcf4d-102">VPN related issues</span></span>

<span data-ttu-id="fcf4d-103">Η επιτυχής υλοποίηση της σύνδεσης VPN για υπολογιστές-πελάτες MDM εξαρτάται από ένα αναπτυγμένο προφίλ που αντικατοπτρίζει σωστά τις απαιτήσεις της υποδομής VPN.</span><span class="sxs-lookup"><span data-stu-id="fcf4d-103">Successful implementation of VPN connectivity for MDM clients depends on a deployed profile that correctly reflects the requirements of the VPN infrastructure.</span></span> <span data-ttu-id="fcf4d-104">Για τις κατάλληλες ρυθμίσεις για τις πλατφόρμες-πελάτες που ερευνάτε, ανατρέξτε στα θέματα:</span><span class="sxs-lookup"><span data-stu-id="fcf4d-104">For the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="fcf4d-105">Ρυθμίσεις ολογραφικών συσκευών των Windows 10 και των Windows για την προσθήκη συνδέσεων VPN με χρήση του Intune</span><span class="sxs-lookup"><span data-stu-id="fcf4d-105">Windows 10 and Windows Holographic device settings to add VPN connections using Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[<span data-ttu-id="fcf4d-106">Προσθήκη ρυθμίσεων VPN σε συσκευές iOS και iPadOS στο Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="fcf4d-106">Add VPN settings on iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-ios)  
[<span data-ttu-id="fcf4d-107">Ρυθμίσεις συσκευής Android για τη ρύθμιση παραμέτρων VPN στο Intune</span><span class="sxs-lookup"><span data-stu-id="fcf4d-107">Android device settings to configure VPN in Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-android)  
[<span data-ttu-id="fcf4d-108">Προσθήκη ρυθμίσεων VPN σε συσκευές macOS στο Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="fcf4d-108">Add VPN settings on macOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

<span data-ttu-id="fcf4d-109">Εάν το προφίλ VPN χρησιμοποιεί έλεγχο ταυτότητας που βασίζεται σε πιστοποιητικό, βεβαιωθείτε ότι τα προφίλ πιστοποιητικού ρίζας και πιστοποιητικού ελέγχου ταυτότητας προγράμματος-πελάτη που συνδέονται με το προφίλ VPN αναπτύσσονται με επιτυχία.</span><span class="sxs-lookup"><span data-stu-id="fcf4d-109">If your VPN profile uses certificate based authentication, make sure that the root certificate and client authentication certificate profiles linked to the VPN profile are deployed successfully.</span></span>

<span data-ttu-id="fcf4d-110">**Κοινά θέματα**</span><span class="sxs-lookup"><span data-stu-id="fcf4d-110">**Common Issues**</span></span>

<span data-ttu-id="fcf4d-111">**Έχω αναπτύξει ένα προφίλ VPN σε μια συσκευή. Intune δείχνει ότι ήταν επιτυχής, αλλά η συσκευή δεν συνδέεται με το VPN.**</span><span class="sxs-lookup"><span data-stu-id="fcf4d-111">**I deployed a VPN profile to a device. Intune is showing that it was successful, but the device is not connecting to the VPN.**</span></span>

<span data-ttu-id="fcf4d-112">Μια επιτυχημένη κατάσταση σημαίνει ότι το Intune έχει αναπτύξει με επιτυχία το προφίλ όπως έχει ρυθμιστεί.</span><span class="sxs-lookup"><span data-stu-id="fcf4d-112">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="fcf4d-113">Ωστόσο, αυτές οι ρυθμίσεις παραμέτρων ενδέχεται να μην συμφωνούν με τις απαιτήσεις του δικτύου ή/και του ελέγχου ταυτότητας.</span><span class="sxs-lookup"><span data-stu-id="fcf4d-113">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="fcf4d-114">Αναθεώρηση αρχεία καταγραφής στην υποδομή και την υπηρεσία ελέγχου ταυτότητας (στο διακομιστή VPN και nps/radius server) για περισσότερες λεπτομέρειες σχετικά με την επιχειρημένη σύνδεση.</span><span class="sxs-lookup"><span data-stu-id="fcf4d-114">Review logs in the infrastructure and authentication service (on the VPN server and NPS/Radius server) for more details about the attempted connection.</span></span> <span data-ttu-id="fcf4d-115">Ίσως χρειαστεί να συνεργαστείτε με την ομάδα υποδομής δικτύου ή τον τρίτο προμηθευτή VPN, για να συγκεντρώσετε και να αναθεωρήσετε αρχεία καταγραφής.</span><span class="sxs-lookup"><span data-stu-id="fcf4d-115">You might need to work with your network infrastructure team, or the third-party VPN vendor, to gather and review logs.</span></span>

<span data-ttu-id="fcf4d-116">**Όταν ρυθμιζοσπάζομαι ένα προσαρμοσμένο VPN για iOS, η δυνατότητα VPN ανά εφαρμογή δεν είναι διαθέσιμη.**</span><span class="sxs-lookup"><span data-stu-id="fcf4d-116">**When I configure a custom VPN for iOS, the per-app VPN feature isn't made available.**</span></span>

<span data-ttu-id="fcf4d-117">Το VPN ανά εφαρμογή για συσκευές iOS στο Intune είναι προς το παρόν διαθέσιμο σε μια συγκεκριμένη λίστα υπηρεσιών παροχής και συνεργατών, οι οποίοι πρέπει επίσης να πληρούν τις προϋποθέσεις πιστοποιητικού πριν από τη ρύθμιση παραμέτρων ενός VPN ανά εφαρμογή.</span><span class="sxs-lookup"><span data-stu-id="fcf4d-117">Per-app VPN for iOS devices in Intune is currently available to a specific list of providers and partners, who must also meet the certificate prerequisites before configuring a per-app VPN.</span></span> <span data-ttu-id="fcf4d-118">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Ρύθμιση εικονικού ιδιωτικού δικτύου (VPN) ανά εφαρμογή για συσκευές iOS/iPadOS στο Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span><span class="sxs-lookup"><span data-stu-id="fcf4d-118">For more info, see [Set up per-app Virtual Private Network (VPN) for iOS/iPadOS devices in Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span></span> 

<span data-ttu-id="fcf4d-119">Για περισσότερες πληροφορίες σχετικά με όλους τους τύπους σύνδεσης VPN στο Intune, ανατρέξτε στο θέμα [Δημιουργία προφίλ VPN για σύνδεση με διακομιστές VPN στο Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="fcf4d-119">For more info about all VPN connection types in Intune, see [Create VPN profiles to connect to VPN servers in Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span></span>  

<span data-ttu-id="fcf4d-120">**Το VPN κατ' απαίτηση του iOS δεν ενεργοποιείται όταν γίνεται πρόσβαση σε έναν ρυθμισμένο τομέα**</span><span class="sxs-lookup"><span data-stu-id="fcf4d-120">**iOS On-Demand VPN is not triggering when a configured domain is accessed**</span></span>

<span data-ttu-id="fcf4d-121">Για να ελέγξετε τις αυτόματες ρυθμίσεις VPN, ορίστε τις ακόλουθες τιμές:</span><span class="sxs-lookup"><span data-stu-id="fcf4d-121">To test automatic VPN settings, set the following values:</span></span>

<span data-ttu-id="fcf4d-122">Θέλω να κάνω τα εξής: **Αξιολόγηση κάθε προσπάθειας σύνδεσης**</span><span class="sxs-lookup"><span data-stu-id="fcf4d-122">I want to do the following: **Evaluate each connection attempt**</span></span> 

<span data-ttu-id="fcf4d-123">Επιλέξτε αν θα συνδεθείτε: **Σύνδεση αν χρειάζεται**</span><span class="sxs-lookup"><span data-stu-id="fcf4d-123">Choose whether to connect: **Connect if needed**</span></span>

<span data-ttu-id="fcf4d-124">Όταν οι χρήστες αποκτούν πρόσβαση σε αυτούς τους τομείς: *όνομα τομέα* **προορισμού**</span><span class="sxs-lookup"><span data-stu-id="fcf4d-124">When users access these domains: **target** *domain name*</span></span>

<span data-ttu-id="fcf4d-125">Εάν η παραπάνω ρύθμιση παραμέτρων δεν είναι επιτυχής, προσθέστε το ακόλουθο στοιχείο:</span><span class="sxs-lookup"><span data-stu-id="fcf4d-125">If the above configuration is not successful, add the following element:</span></span>

<span data-ttu-id="fcf4d-126">Όταν δεν είναι δυνατή η πρόσβαση σε αυτήν τη διεύθυνση URL, επιβάλλετε τη σύνδεση του VPN: **BADURL**</span><span class="sxs-lookup"><span data-stu-id="fcf4d-126">When this URL is unreachable, force connect the VPN: **BADURL**</span></span>