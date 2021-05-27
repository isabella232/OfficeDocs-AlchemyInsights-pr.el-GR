---
title: Η αντιμετώπιση προβλημάτων του ediscovery περιέχει σφάλματα
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 1df2b7153cac99419adc4f72b1c3732e7c746eac
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 05/20/2021
ms.locfileid: "52676149"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a><span data-ttu-id="6f08d-102">Η αντιμετώπιση προβλημάτων του ediscovery περιέχει σφάλματα</span><span class="sxs-lookup"><span data-stu-id="6f08d-102">Troubleshooting ediscovery holds errors</span></span>

<span data-ttu-id="6f08d-103">Αντιμετωπίζετε προβλήματα με τις κάτοχοι του eDiscovery;</span><span class="sxs-lookup"><span data-stu-id="6f08d-103">Experiencing issues with eDiscovery holds?</span></span> <span data-ttu-id="6f08d-104">Ακολουθούν ορισμένες βέλτιστες πρακτικές που πρέπει να λάβετε υπόψη:</span><span class="sxs-lookup"><span data-stu-id="6f08d-104">Here are some best practices to consider:</span></span>

- <span data-ttu-id="6f08d-105">Ελέγξτε την κατάσταση διανομής αναμονής.</span><span class="sxs-lookup"><span data-stu-id="6f08d-105">Check the hold distribution status.</span></span>  <span data-ttu-id="6f08d-106">Εάν η κατάσταση είναι **"Σε εκκρεμότητα"** ή **"Απενεργοποιημένη" (Σε εκκρεμότητα),** περιμένετε να ολοκληρωθεί η διανομή αναμονής.</span><span class="sxs-lookup"><span data-stu-id="6f08d-106">If status is **On (Pending)** or **Off (Pending)**, wait for hold distribution to complete.</span></span>
- <span data-ttu-id="6f08d-107">Συγχώνευση eDiscovery κρατήστε τις ενημερώσεις σε μια μεμονωμένη μαζική αίτηση αντί να ενημερώνετε την πολιτική επανειλημμένα για κάθε συναλλαγή.</span><span class="sxs-lookup"><span data-stu-id="6f08d-107">Merge eDiscovery hold updates into a single bulk request instead of updating the policy repeatedly for each transaction.</span></span>
- <span data-ttu-id="6f08d-108">Εκτελέστε Set-CaseHoldPolicy <policyname> -RetryDistribution στο Powershell του Κέντρου ασφάλειας και συμμόρφωσης.</span><span class="sxs-lookup"><span data-stu-id="6f08d-108">Run Set-CaseHoldPolicy <policyname> -RetryDistribution in the Security and Compliance Center Powershell.</span></span> <span data-ttu-id="6f08d-109">Για λεπτομέρειες, ανατρέξτε [Σύνδεση στο Κέντρο ασφάλειας & PowerShell.](/powershell/exchange/connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="6f08d-109">For details, see [Connect to Security & Compliance Center PowerShell](/powershell/exchange/connect-to-scc-powershell).</span></span>

<span data-ttu-id="6f08d-110">Για τα βήματα για να ελέγξετε αυτές τις ρυθμίσεις και πρόσθετες βέλτιστες πρακτικές για την αντιμετώπιση και την επίλυση προβλημάτων που περιέχει το eDiscovery, ανατρέξτε στο θέμα Αντιμετώπιση σφαλμάτων διατήρησης [του eDiscovery.](/microsoft-365/compliance/hold-distribution-errors)</span><span class="sxs-lookup"><span data-stu-id="6f08d-110">For steps to check these settings and additional best practices for mitigating and resolving eDiscovery holds issues, see [Troubleshoot eDiscovery hold errors](/microsoft-365/compliance/hold-distribution-errors).</span></span>
<span data-ttu-id="6f08d-111">Για πληροφορίες σχετικά με την αντιμετώπιση άλλων συνηθισμένων ζητημάτων eDiscovery, ανατρέξτε στο θέμα Διερεύνηση, αντιμετώπιση προβλημάτων και [επίλυση κοινών ζητημάτων eDiscovery.](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues)</span><span class="sxs-lookup"><span data-stu-id="6f08d-111">For info about troubleshooting other common eDiscovery issues, see [Investigate, troubleshoot, and resolve common eDiscovery issues](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).</span></span>
