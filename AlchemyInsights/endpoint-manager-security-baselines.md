---
title: EndPoint Manager - Γραμμές βάσης ασφαλείας
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
ms.openlocfilehash: d2a063fdc4929cbee5fef71bfb47ace8f2ba458f
ms.sourcegitcommit: 430d247cb5dd5dc5d1f82d977456558dfd514277
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51420879"
---
# <a name="endpoint-manager---security-baselines"></a><span data-ttu-id="4d89b-102">EndPoint Manager - Γραμμές βάσης ασφαλείας</span><span class="sxs-lookup"><span data-stu-id="4d89b-102">EndPoint Manager - Security baselines</span></span>

<span data-ttu-id="4d89b-103">Οι γραμμές βάσης ασφαλείας είναι προ-ρυθμισμένες ομάδες ρυθμίσεων των Windows που σας βοηθούν να εφαρμόσετε τις ρυθμίσεις ασφαλείας που συνιστώνται από τις σχετικές ομάδες ασφαλείας.</span><span class="sxs-lookup"><span data-stu-id="4d89b-103">Security baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams.</span></span> <span data-ttu-id="4d89b-104">Αυτές οι γραμμές βάσης μπορούν να προσαρμοστούν ώστε να παρέχουν μόνο τις ρυθμίσεις και τις τιμές που θέλετε.</span><span class="sxs-lookup"><span data-stu-id="4d89b-104">These baselines can be customized to deliver only the settings and values desired.</span></span> <span data-ttu-id="4d89b-105">Για περισσότερες πληροφορίες σχετικά με τις γραμμές βάσης ασφαλείας, ανατρέξτε στο θέμα Χρήση γραμμών [βάσης ασφαλείας για τη ρύθμιση παραμέτρων συσκευών Windows 10 στο Intune.](https://docs.microsoft.com/mem/intune/protect/security-baselines)</span><span class="sxs-lookup"><span data-stu-id="4d89b-105">For more information about security baselines, see [Use security baselines to configure Windows 10 devices in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span></span>

<span data-ttu-id="4d89b-106">Υπάρχουν επί του παρόντος γραμμές βάσης για αυτά τα προϊόντα:</span><span class="sxs-lookup"><span data-stu-id="4d89b-106">There are currently baselines for these products:</span></span>

- <span data-ttu-id="4d89b-107">Ρυθμίσεις ασφαλείας του Windows MDM</span><span class="sxs-lookup"><span data-stu-id="4d89b-107">Windows MDM Security settings</span></span>
- <span data-ttu-id="4d89b-108">Microsoft Defender για την ασφάλεια του EndPoint</span><span class="sxs-lookup"><span data-stu-id="4d89b-108">Microsoft Defender for EndPoint Security</span></span>
- <span data-ttu-id="4d89b-109">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="4d89b-109">Microsoft Edge</span></span>

<span data-ttu-id="4d89b-110">Κάθε μία από τις γραμμές βάσης ενημερώνεται περιοδικά και κυκλοφορεί σε τμηματικές εκδόσεις.</span><span class="sxs-lookup"><span data-stu-id="4d89b-110">Each of the baselines are updated periodically and released in incremental versions.</span></span> <span data-ttu-id="4d89b-111">Κάθε έκδοση προσθέτει και καταργεί ρυθμίσεις από την προηγούμενη έκδοση για να εξασφαλίσει ότι η γραμμή βάσης πληροί τις τρέχουσες οδηγίες.</span><span class="sxs-lookup"><span data-stu-id="4d89b-111">Each version adds and or removes settings from the previous version to ensure that the baseline meets current guidance.</span></span> <span data-ttu-id="4d89b-112">Η κονσόλα γραμμών βάσης ασφαλείας στην Ασφάλεια τελικού σημείου επιτρέπει τη σύγκριση διαφορετικών εκδόσεων, κάνοντας ορατές τις αλλαγές από την έκδοση στην έκδοση.</span><span class="sxs-lookup"><span data-stu-id="4d89b-112">The Security baselines console in Endpoint Security allows different versions to be compared by making the changes from version to version visible.</span></span>

<span data-ttu-id="4d89b-113">Για οδηγίες σχετικά με τον τρόπο με τον οποίο μπορείτε να αλλάξετε πιο αποτελεσματικά την έκδοση της γραμμής βάσης που αναπτύσσεται, ανατρέξτε στο θέμα Διαχείριση προφίλ [γραμμής βάσης ασφαλείας στο Microsoft Intune.](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure)</span><span class="sxs-lookup"><span data-stu-id="4d89b-113">For guidance on how to most effectively change which version of baseline is deployed, see [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span></span>

<span data-ttu-id="4d89b-114">Μετά την ανάπτυξη μιας γραμμής βάσης ασφαλείας, μπορείτε να παρακολουθείτε την κατάσταση της ανάπτυξης και να αναθεωρήσετε τις ρυθμίσεις ανά συσκευή.</span><span class="sxs-lookup"><span data-stu-id="4d89b-114">After deploying a security baseline, you can monitor the state of deployment and review settings on a device-by-device basis.</span></span>

<span data-ttu-id="4d89b-115">**Σημείωση:** Τα δεδομένα αναφοράς για τις γραμμές βάσης μπορεί να διαρκέσει έως και 24 ώρες για να εμφανιστούν από την αρχική ανάπτυξη σε μια συσκευή και έως και 6 ώρες για περαιτέρω ενημερώσεις.</span><span class="sxs-lookup"><span data-stu-id="4d89b-115">**Note:** The reporting data for baselines may take up to 24 hours to appear from the initial deployment to a device and up to 6 hours for further updates.</span></span> 

<span data-ttu-id="4d89b-116">Η πιο συνηθισμένη αιτία μιας ρύθμισης γραμμής βάσης που δεν εφαρμόζεται είναι επειδή η ίδια ρύθμιση χρησιμοποιείται σε διαφορετικό προφίλ.</span><span class="sxs-lookup"><span data-stu-id="4d89b-116">The most common cause of a baseline setting not applying is because the same setting being used in a different profile.</span></span> <span data-ttu-id="4d89b-117">Αυτό το σενάριο μπορεί να διερευνηθεί για συγκεκριμένη συσκευή, επιλέγοντας τη συγκεκριμένη συσκευή μέσα από τον κόμβο κατάστασης συσκευής του προφίλ γραμμής βάσης ασφαλείας.</span><span class="sxs-lookup"><span data-stu-id="4d89b-117">This scenario can be investigated for specific device by selecting that device from within the Device Status node of the Security Baseline profile.</span></span> <span data-ttu-id="4d89b-118">Για λεπτομέρειες, ανατρέξτε [στο θέμα Επίλυση διενέξεων για γραμμές βάσης ασφαλείας.](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines)</span><span class="sxs-lookup"><span data-stu-id="4d89b-118">For details, see [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span></span>