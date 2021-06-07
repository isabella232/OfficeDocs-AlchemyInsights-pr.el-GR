---
title: Προβλήματα επιδόσεων για τον Microsoft Defender για το Τελικό σημείο σε Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793757"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a><span data-ttu-id="f9660-102">Προβλήματα επιδόσεων για τον Microsoft Defender για το Τελικό σημείο σε Linux</span><span class="sxs-lookup"><span data-stu-id="f9660-102">Performance issues for Microsoft Defender for Endpoint on Linux</span></span>

<span data-ttu-id="f9660-103">Αυτό το άρθρο σάς καθοδηγεί στα βήματα για τον προσδιορισμό ζητημάτων επιδόσεων για τον Microsoft Defender για το Τελικό σημείο σε Linux.</span><span class="sxs-lookup"><span data-stu-id="f9660-103">This article guides you through the steps of identifying performance issues for Microsoft Defender for Endpoint on Linux.</span></span>

<span data-ttu-id="f9660-104">Είναι σημαντικό να επαληθεύσετε πρώτα ότι το πρόβλημα που αντιμετωπίζετε έχει επιλυθεί με την [πιο πρόσφατη έκδοση.](/microsoft-365/security/defender-endpoint/linux-whatsnew)</span><span class="sxs-lookup"><span data-stu-id="f9660-104">It's important to first verify that the problem you're experiencing is resolved with the [latest version](/microsoft-365/security/defender-endpoint/linux-whatsnew).</span></span> 

<span data-ttu-id="f9660-105">Για να ξεκινήσετε την έρευνα, ανατρέξτε [στο θέμα Αντιμετώπιση προβλημάτων επιδόσεων για τον Microsoft Defender για το Τελικό σημείο σε Linux.](/microsoft-365/security/defender-endpoint/linux-support-perf)</span><span class="sxs-lookup"><span data-stu-id="f9660-105">To start your investigation, see [Troubleshoot performance issues for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-support-perf).</span></span>

## <a name="exclusions"></a><span data-ttu-id="f9660-106">Εξαιρέσεις</span><span class="sxs-lookup"><span data-stu-id="f9660-106">Exclusions</span></span>

<span data-ttu-id="f9660-107">Οι εξαιρέσεις μπορούν να σας βοηθήσουν να μετριάσουν τα προβλήματα επιδόσεων.</span><span class="sxs-lookup"><span data-stu-id="f9660-107">Exclusions can help to mitigate performance issues.</span></span> <span data-ttu-id="f9660-108">Ελέγξτε τις εξαιρέσεις σας πριν ξεκινήσετε, ώστε να είναι γνωστός και τεκμηριωμένος οποιοσδήποτε πρόσθετος κίνδυνος.</span><span class="sxs-lookup"><span data-stu-id="f9660-108">Review your exclusions before you begin so any additional risk is known and documented.</span></span>

<span data-ttu-id="f9660-109">Για περισσότερες πληροφορίες, ανατρέξτε στο [θέμα Ρύθμιση παραμέτρων και επικύρωση εξαιρέσεων για το Microsoft Defender για τελικό σημείο σε Linux.](/microsoft-365/security/defender-endpoint/linux-exclusions)</span><span class="sxs-lookup"><span data-stu-id="f9660-109">For more information, see [Configure and validate exclusions for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-exclusions).</span></span>

<span data-ttu-id="f9660-110">Όταν έχετε πολλά αρχεία που & να εξαιρέσετε και βρίσκονται όλα στο ίδιο σημείο τοποθέτησης, ίσως είναι ευκολότερο να εξαιρέσετε το σημείο τοποθέτησης.</span><span class="sxs-lookup"><span data-stu-id="f9660-110">When you have multiple files & folders to exclude and they're all on the same mountpoint, it might be easier to exclude the mountpoint.</span></span> <span data-ttu-id="f9660-111">Ξεκινώντας από την έκδοση 101.22.80 του Φεβρουαρίου, μπορείτε να εξαιρέσετε ένα ολόκληρο σημείο τοποθέτησης.</span><span class="sxs-lookup"><span data-stu-id="f9660-111">Starting with February release 101.22.80, you can exclude an entire mountpoint.</span></span>

<span data-ttu-id="f9660-112">Για παράδειγμα, εάν το /mnt/backup είναι ένα σημείο τοποθέτησης, μπορείτε να προσθέσετε /mnt/backup στη λίστα εξαιρέσεων εκτελώντας αυτή την εντολή:</span><span class="sxs-lookup"><span data-stu-id="f9660-112">For example, if /mnt/backup is a mountpoint, you can add /mnt/backup to the exclude list by running this command:</span></span>

`$ mdatp exclusion folder add –path /mnt/backup`

<span data-ttu-id="f9660-113">**Σημείωση:** Η προσθήκη εξαιρέσεων αυξάνει τον κίνδυνο να μην εντοπιστεί λογισμικό κακόβουλης λειτουργίας και θα πρέπει να γίνεται χειρισμός και να εφαρμόζεται με προσοχή.</span><span class="sxs-lookup"><span data-stu-id="f9660-113">**Note**: Adding exclusions increases the risk of malware not being detected and should be handled and implemented with care.</span></span>

## <a name="need-help"></a><span data-ttu-id="f9660-114">Χρειάζεστε βοήθεια;</span><span class="sxs-lookup"><span data-stu-id="f9660-114">Need Help?</span></span>

<span data-ttu-id="f9660-115">Για να σας βοηθήσει με τον πιο αποτελεσματικό τρόπο, συλλέξτε τα διαγνωστικά δεδομένα πριν ανοίξετε μια υπόθεση υποστήριξης.</span><span class="sxs-lookup"><span data-stu-id="f9660-115">To assist you in the most efficient way, collect the diagnostic data before opening a support case.</span></span>
