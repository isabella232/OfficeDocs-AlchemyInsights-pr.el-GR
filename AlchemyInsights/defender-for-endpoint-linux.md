---
title: Microsoft Defender για τελικό σημείο σε Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11490"
- "9001464"
ms.openlocfilehash: 99894d83c51e11ea6dd1746568762eac856306b3
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/02/2021
ms.locfileid: "52731679"
---
# <a name="microsoft-defender-for-endpoint-on-linux"></a><span data-ttu-id="16be2-102">Microsoft Defender για τελικό σημείο σε Linux</span><span class="sxs-lookup"><span data-stu-id="16be2-102">Microsoft Defender for Endpoint on Linux</span></span>

<span data-ttu-id="16be2-103">Για λεπτομερή τεκμηρίωση του Linux, ανατρέξτε στο [θέμα Microsoft Defender για τελικό σημείο σε Linux.](/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint-linux)</span><span class="sxs-lookup"><span data-stu-id="16be2-103">For detailed Linux documentation, see [Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint-linux).</span></span>

<span data-ttu-id="16be2-104">Για πληροφορίες σχετικά με το σύστημα και την εγκατάσταση, ανατρέξτε στο θέμα:</span><span class="sxs-lookup"><span data-stu-id="16be2-104">For system and installation information, see:</span></span>

- [<span data-ttu-id="16be2-105">Προαπαιτούμενα</span><span class="sxs-lookup"><span data-stu-id="16be2-105">Prerequisites</span></span>](/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint-linux#prerequisites)
- [<span data-ttu-id="16be2-106">Απαιτήσεις συστήματος</span><span class="sxs-lookup"><span data-stu-id="16be2-106">System requirements</span></span>](/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint-linux#system-requirements)
- [<span data-ttu-id="16be2-107">Οδηγίες εγκατάστασης</span><span class="sxs-lookup"><span data-stu-id="16be2-107">Installation instructions</span></span>](/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint-linux#installation-instructions)
- [<span data-ttu-id="16be2-108">Συνδέσεις δικτύου</span><span class="sxs-lookup"><span data-stu-id="16be2-108">Network connections</span></span>](/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint-linux#network-connections)

<span data-ttu-id="16be2-109">Για οδηγίες, ανατρέξτε στο θέμα:</span><span class="sxs-lookup"><span data-stu-id="16be2-109">For instructions, see:</span></span>

- [<span data-ttu-id="16be2-110">Ρύθμιση παραμέτρων διακομιστή μεσολάβησης συσκευής και συνδεσιμότητας Στο Internet</span><span class="sxs-lookup"><span data-stu-id="16be2-110">Configure device proxy and Internet connectivity settings</span></span>](/microsoft-365/security/defender-endpoint/configure-proxy-internet#enable-access-to-microsoft-defender-atp-service-urls-in-the-proxy-server)
- [<span data-ttu-id="16be2-111">Ανάπτυξη ενημερώσεων για τον Microsoft Defender για το Τελικό σημείο σε Linux</span><span class="sxs-lookup"><span data-stu-id="16be2-111">Deploy updates for Microsoft Defender for Endpoint on Linux</span></span>](/microsoft-365/security/defender-endpoint/linux-updates)
- [<span data-ttu-id="16be2-112">Τρόπος ρύθμισης παραμέτρων του Microsoft Defender για το Τελικό σημείο σε Linux</span><span class="sxs-lookup"><span data-stu-id="16be2-112">How to configure Microsoft Defender for Endpoint on Linux</span></span>](/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint-linux#how-to-configure-microsoft-defender-for-endpoint-on-linux)
- [<span data-ttu-id="16be2-113">Υποστηριζόμενες εντολές</span><span class="sxs-lookup"><span data-stu-id="16be2-113">Supported commands</span></span>](/microsoft-365/security/defender-endpoint/linux-resources#supported-commands)

## <a name="i-need-help"></a><span data-ttu-id="16be2-114">Χρειάζομαι βοήθεια!</span><span class="sxs-lookup"><span data-stu-id="16be2-114">I need help!</span></span>

<span data-ttu-id="16be2-115">Εάν δεν μπορείτε να βρείτε τις πληροφορίες/βοήθεια που αναζητάτε, περιορίστε τη συμβολοσειρά αναζήτησης.</span><span class="sxs-lookup"><span data-stu-id="16be2-115">If you can't find the information/help you're looking for, refine your search string.</span></span>

<span data-ttu-id="16be2-116">Πριν επικοινωνήσετε με την Υποστήριξη της Microsoft, φροντίστε να συλλέξετε τα δεδομένα που απαιτούνται για να διερευνήσετε το πρόβλημα και να τα επισυνάψετε στο δελτίο.</span><span class="sxs-lookup"><span data-stu-id="16be2-116">Before contacting Microsoft Support, make sure to collect the data required to investigate your issue, and attach it to the ticket.</span></span> <span data-ttu-id="16be2-117">Για τα βήματα για τη συλλογή των πληροφοριών διάγνωσης, ανατρέξτε στο θέμα [Συλλογή διαγνωστικών δεδομένων.](/microsoft-365/security/defender-endpoint/linux-resources#collect-diagnostic-information)</span><span class="sxs-lookup"><span data-stu-id="16be2-117">For steps to collect the diagnosic information, see [Collect diagnostic data](/microsoft-365/security/defender-endpoint/linux-resources#collect-diagnostic-information).</span></span>