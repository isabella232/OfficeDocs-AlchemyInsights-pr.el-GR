---
title: Οι ενδείξεις δεν λειτουργούν με το πρόγραμμα περιήγησης Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11230"
- "9005470"
ms.openlocfilehash: df62d965e0dc2ddb656571af99b1e4c3cb52ea35
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676241"
---
# <a name="indicators-dont-work-using-edge-browser"></a><span data-ttu-id="b1140-102">Οι ενδείξεις δεν λειτουργούν με το πρόγραμμα περιήγησης Edge</span><span class="sxs-lookup"><span data-stu-id="b1140-102">Indicators don't work using Edge browser</span></span>

<span data-ttu-id="b1140-103">Μετά τη δημιουργία μιας Ένδειξης, δεν τιμάται από τον Edge (Smartscreen).</span><span class="sxs-lookup"><span data-stu-id="b1140-103">After you created an Indicator, it's not honored by Edge (Smartscreen).</span></span> <span data-ttu-id="b1140-104">Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα Δημιουργία δεικτών για IPs και διευθύνσεις URL/τομείς.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)</span><span class="sxs-lookup"><span data-stu-id="b1140-104">For more information, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>

## <a name="step-1-ensure-the-following"></a><span data-ttu-id="b1140-105">Βήμα 1: Εξασφαλίστε τα εξής</span><span class="sxs-lookup"><span data-stu-id="b1140-105">Step 1: Ensure the following</span></span>

- <span data-ttu-id="b1140-106">Βεβαιωθείτε ότι η ένδειξη είναι σωστή (δεν υπάρχουν λάθη στη διεύθυνση IP/URL, σωστή ενέργεια, οι σωστές ομάδες RBAC).</span><span class="sxs-lookup"><span data-stu-id="b1140-106">Verify that the indicator is correct (no typos in IP/URL, correct action, the correct RBAC groups).</span></span>
- <span data-ttu-id="b1140-107">Περιμένετε τουλάχιστον 2 ώρες μετά τη δημιουργία της ένδειξης για να ληφθεί υπόψη τυχόν λανθάνων χρόνος.</span><span class="sxs-lookup"><span data-stu-id="b1140-107">Wait the minimum 2 hours after creating the indicator to take into account any possible latency.</span></span>
- <span data-ttu-id="b1140-108">Επιβεβαιώστε ότι τα συστήματα έχουν επιβεβαιωθεί στον Microsoft Defender για το τελικό σημείο.</span><span class="sxs-lookup"><span data-stu-id="b1140-108">Confirm that the system(s) are onboarded to Microsoft Defender for Endpoint.</span></span>
- <span data-ttu-id="b1140-109">Βεβαιωθείτε ότι τα συστήματα μπορούν να επικοινωνούν με το Cloud.</span><span class="sxs-lookup"><span data-stu-id="b1140-109">Verify that system(s) can communicate with the Cloud.</span></span>
- <span data-ttu-id="b1140-110">Βεβαιωθείτε ότι το Smartscreen είναι ενεργοποιημένο και προσβάσιμο, από την τοποθεσία [δοκιμής.](https://demo.smartscreen.msft.net)</span><span class="sxs-lookup"><span data-stu-id="b1140-110">Verify that Smartscreen is enabled and reachable by going to the [test site](https://demo.smartscreen.msft.net).</span></span>

## <a name="step-2-troubleshoot-the-potential-issue"></a><span data-ttu-id="b1140-111">Βήμα 2: Αντιμετώπιση του πιθανού προβλήματος</span><span class="sxs-lookup"><span data-stu-id="b1140-111">Step 2: Troubleshoot the potential issue</span></span>

- <span data-ttu-id="b1140-112">Βεβαιωθείτε ότι το πρόγραμμα-πελάτης πληροί τις απαιτήσεις.</span><span class="sxs-lookup"><span data-stu-id="b1140-112">Make sure the client meets the requirements.</span></span> <span data-ttu-id="b1140-113">Για λεπτομέρειες, [ανατρέξτε στο θέμα Δημιουργία δεικτών για IPs και διευθύνσεις URL/τομείς.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)</span><span class="sxs-lookup"><span data-stu-id="b1140-113">For details, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>
- <span data-ttu-id="b1140-114">Βεβαιωθείτε ότι χρησιμοποιείτε την πιο πρόσφατη έκδοση του προγράμματος περιήγησης Edge.</span><span class="sxs-lookup"><span data-stu-id="b1140-114">Make sure you're running the latest version of the Edge browser.</span></span> <span data-ttu-id="b1140-115">Για να μάθετε την πιο πρόσφατη έκδοση, [ανατρέξτε στο θέμα Μάθετε ποια έκδοση Microsoft Edge που έχετε.](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb)</span><span class="sxs-lookup"><span data-stu-id="b1140-115">To find out the latest version, see [Find out which version of Microsoft Edge you have](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).</span></span>
- <span data-ttu-id="b1140-116">Επανεκκινήστε το πρόγραμμα περιήγησης Edge.</span><span class="sxs-lookup"><span data-stu-id="b1140-116">Restart the Edge browser.</span></span>
- <span data-ttu-id="b1140-117">Μεταβείτε στην τοποθεσία για την οποία έχετε ρυθμίσει μια ένδειξη.</span><span class="sxs-lookup"><span data-stu-id="b1140-117">Navigate to the site for which you have setup an indicator.</span></span> <span data-ttu-id="b1140-118">Εάν η τοποθεσία δεν εμφανίζεται όπως αναμένεται, συνεχίστε στο βήμα 3.</span><span class="sxs-lookup"><span data-stu-id="b1140-118">If the site does not appear as expected, continue to Step 3.</span></span> 

## <a name="step-3-collect-data"></a><span data-ttu-id="b1140-119">Βήμα 3: Συλλογή δεδομένων</span><span class="sxs-lookup"><span data-stu-id="b1140-119">Step 3: Collect data</span></span>

- <span data-ttu-id="b1140-120">Συλλέξτε **διαγνωστικά δεδομένα MDEClientAnalyzer.**</span><span class="sxs-lookup"><span data-stu-id="b1140-120">Collect **MDEClientAnalyzer** diagnostic data.</span></span> <span data-ttu-id="b1140-121">Για οδηγίες, [ανατρέξτε στο θέμα Προβλήματα με τους υπολογιστές που είναι σε θέση να ενταφιούν στον Microsoft Defender για το τελικό σημείο.](issues-with-onboarding-machines.md)</span><span class="sxs-lookup"><span data-stu-id="b1140-121">For instructions, see [Issues with onboarding machines to Microsoft Defender for Endpoint](issues-with-onboarding-machines.md).</span></span>
- <span data-ttu-id="b1140-122">Εάν είστε άνετα να εγκαταστήσετε και να συλλέξετε μια ανίχνευση Fiddler, [ανατρέξτε στο θέμα Telerik Fiddler.](http://www.telerik.com/fiddler)</span><span class="sxs-lookup"><span data-stu-id="b1140-122">If you are comfortable installing and collecting a Fiddler trace, see [Telerik Fiddler](http://www.telerik.com/fiddler).</span></span>
- <span data-ttu-id="b1140-123">Εάν προτιμάτε οδηγίες από την Υποστήριξη της Microsoft, επιλέξτε το εικονίδιο υποστήριξης παρακάτω για να ανοίξετε μια υπόθεση υποστήριξης.</span><span class="sxs-lookup"><span data-stu-id="b1140-123">If you prefer guidance from Microsoft Support, select the Support icon below to open a support case.</span></span>
