---
title: Κανόνες μείωσης επιφάνειας επίθεσης
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
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676231"
---
# <a name="attack-surface-reduction-rules"></a><span data-ttu-id="ec66d-102">Κανόνες μείωσης επιφάνειας επίθεσης</span><span class="sxs-lookup"><span data-stu-id="ec66d-102">Attack surface reduction rules</span></span>

<span data-ttu-id="ec66d-103">Η εξαίρεση αρχείων ή φακέλων μπορεί να μειώσει σημαντικά την προστασία που παρέχεται από τους κανόνες μείωσης επιφάνειας επίθεσης.</span><span class="sxs-lookup"><span data-stu-id="ec66d-103">Excluding files or folders can severely reduce the protection provided by attack surface reduction rules.</span></span> <span data-ttu-id="ec66d-104">Τα αρχεία που θα είχαν αποκλειστεί από έναν κανόνα επιτρέπεται να εκτελούνται και δεν καταγράφεται αναφορά ή συμβάν.</span><span class="sxs-lookup"><span data-stu-id="ec66d-104">Files that would have been blocked by a rule are allowed to run, and no report or event is recorded.</span></span> <span data-ttu-id="ec66d-105">Μια εξαίρεση ισχύει για όλους τους κανόνες που επιτρέπουν εξαιρέσεις.</span><span class="sxs-lookup"><span data-stu-id="ec66d-105">An exclusion applies to all rules that allow exclusions.</span></span>

<span data-ttu-id="ec66d-106">Οι εξαιρέσεις ASR χρησιμοποιούν την ίδια σύνταξη με Προστασία του Microsoft Defender από ιούς εξαιρέσεων.</span><span class="sxs-lookup"><span data-stu-id="ec66d-106">ASR exclusions use the same syntax as Microsoft Defender Antivirus exclusions.</span></span> <span data-ttu-id="ec66d-107">Για λεπτομέρειες, ανατρέξτε [στο θέμα Ρύθμιση παραμέτρων και επικύρωση εξαιρέσεων για Προστασία του Microsoft Defender από ιούς σαρώσεις.](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="ec66d-107">For details, see [Configure and validate exclusions for Microsoft Defender Antivirus scans](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus).</span></span> <span data-ttu-id="ec66d-108">Για να αποφύγετε προβλήματα, εξετάστε [τα κοινά λάθη για να αποφύγετε κατά τον ορισμό εξαιρέσεων.](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="ec66d-108">To avoid problems, review [Common mistakes to avoid when defining exclusions](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="ec66d-109">Δεν υποστηρίζουν όλοι οι κανόνες ASR τις εξαιρέσεις.</span><span class="sxs-lookup"><span data-stu-id="ec66d-109">Not all ASR rules support exclusions.</span></span> <span data-ttu-id="ec66d-110">Για να επαληθεύσετε εάν ο κανόνας σας υποστηρίζει εξαιρέσεις, ανατρέξτε στον πίνακα [Κανόνες μείωσης επιφάνειας επίθεσης.](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)</span><span class="sxs-lookup"><span data-stu-id="ec66d-110">To validate if your rule supports exclusions, see the table [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

## <a name="attack-surface-reduction-rules"></a><span data-ttu-id="ec66d-111">Κανόνες μείωσης επιφάνειας επίθεσης</span><span class="sxs-lookup"><span data-stu-id="ec66d-111">Attack surface reduction rules</span></span>

<span data-ttu-id="ec66d-112">Η επιφάνεια επίθεσης του οργανισμού σας περιλαμβάνει όλα τα σημεία όπου ένας εισβολέας θα μπορούσε να θέσει σε κίνδυνο τις συσκευές ή τα δίκτυα του οργανισμού.</span><span class="sxs-lookup"><span data-stu-id="ec66d-112">Your organization attack surface includes all the places where an attacker could compromise organization devices or networks.</span></span> <span data-ttu-id="ec66d-113">Η μείωση της επιφάνειας της επίθεσης σημαίνει ότι προστατεύετε τις συσκευές και το δίκτυο της εταιρείας, γεγονός που αφήνει τους επιτιθέμενους με λιγότερους τρόπους για να εκτελέσουν επιθέσεις.</span><span class="sxs-lookup"><span data-stu-id="ec66d-113">Reducing your attack surface means protecting the organization devices and network, which leaves attackers with fewer ways to perform attacks.</span></span> <span data-ttu-id="ec66d-114">Η ρύθμιση παραμέτρων των κανόνων μείωσης επιφάνειας επίθεσης στο Microsoft Defender για το τελικό σημείο μπορεί να σας βοηθήσει.</span><span class="sxs-lookup"><span data-stu-id="ec66d-114">Configuring attack surface reduction rules in Microsoft Defender for Endpoint can help.</span></span>

<span data-ttu-id="ec66d-115">Για περισσότερες πληροφορίες, ανατρέξτε στα θέματα:</span><span class="sxs-lookup"><span data-stu-id="ec66d-115">For more information, see:</span></span>

- [<span data-ttu-id="ec66d-116">Αντιστοίχιση GUID κανόνα ASR με όνομα</span><span class="sxs-lookup"><span data-stu-id="ec66d-116">Map ASR rule GUID to name</span></span>](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- <span data-ttu-id="ec66d-117">Απαιτήσεις κανόνων ASR:</span><span class="sxs-lookup"><span data-stu-id="ec66d-117">ASR rules requirements:</span></span>
    - [<span data-ttu-id="ec66d-118">Windows 10 Pro, έκδοση 1709 ή νεότερη</span><span class="sxs-lookup"><span data-stu-id="ec66d-118">Windows 10 Pro, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="ec66d-119">Windows 10 Enterprise, έκδοση 1709 ή νεότερη</span><span class="sxs-lookup"><span data-stu-id="ec66d-119">Windows 10 Enterprise, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="ec66d-120">Windows Διακομιστής, έκδοση 1803 (Εξαμηνιό κανάλι) ή νεότερη</span><span class="sxs-lookup"><span data-stu-id="ec66d-120">Windows Server, version 1803 (Semi-Annual Channel) or later</span></span>](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a><span data-ttu-id="ec66d-121">Προσδιορισμός της σωστής εξαίρεσης που θα εφαρμοστεί</span><span class="sxs-lookup"><span data-stu-id="ec66d-121">Identify the correct exclusion to apply</span></span>

1. <span data-ttu-id="ec66d-122">Αναζητήστε το eventID 1121 ή 1122 στο αρχείο καταγραφής microsoft-Windows-Windows Defender/Λειτουργικό αρχείο καταγραφής.</span><span class="sxs-lookup"><span data-stu-id="ec66d-122">Look for eventID 1121 or 1122 in the Microsoft-Windows-Windows Defender/Operational log.</span></span>

1. <span data-ttu-id="ec66d-123">Αξιολογήστε το σενάριο αποκλεισμού και το περιβάλλον και επιβεβαιώστε ότι αυτό το σενάριο πρέπει να ξεμπλοκάρει.</span><span class="sxs-lookup"><span data-stu-id="ec66d-123">Evaluate the block scenario and context and confirm that this scenario needs to be unblocked.</span></span>

1. <span data-ttu-id="ec66d-124">Διαβάστε την τιμή "Διαδρομή" στις λεπτομέρειες του συμβάντος, η οποία είναι η τιμή που καθορίζει την εξαίρεση.</span><span class="sxs-lookup"><span data-stu-id="ec66d-124">Read the Path value in the event details, which is the value that defines the exclusion.</span></span>
    - <span data-ttu-id="ec66d-125">Κάντε την εξαίρεση όσο το δυνατόν πιο αυστηρή.</span><span class="sxs-lookup"><span data-stu-id="ec66d-125">Make the exclusion as strict as possible.</span></span>
    - <span data-ttu-id="ec66d-126">Εφαρμόστε έναν χαρακτήρες μπαλαντέρ όπου χρειάζεται (για παράδειγμα, αντικατάσταση μεταβλητής χρήστη).</span><span class="sxs-lookup"><span data-stu-id="ec66d-126">Apply a wildcard where needed (for example, replace User variable).</span></span>

1. <span data-ttu-id="ec66d-127">Εφαρμόστε την εξαίρεση σύμφωνα με τις ανάγκες ανάπτυξης.</span><span class="sxs-lookup"><span data-stu-id="ec66d-127">Apply the exclusion according to your deployment needs.</span></span> <span data-ttu-id="ec66d-128">Για λεπτομέρειες, ανατρέξτε στο θέμα [Προσαρμογή κανόνων μείωσης επιφάνειας επίθεσης.](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction)</span><span class="sxs-lookup"><span data-stu-id="ec66d-128">For details, see [Customize attack surface reduction rules](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).</span></span>

## <a name="exclusion-is-not-honored"></a><span data-ttu-id="ec66d-129">Ο αποκλεισμός δεν τιμάται</span><span class="sxs-lookup"><span data-stu-id="ec66d-129">Exclusion is not honored</span></span>

1. <span data-ttu-id="ec66d-130">Προσδιορίστε εάν ο κανόνας υποστηρίζει εξαιρέσεις.</span><span class="sxs-lookup"><span data-stu-id="ec66d-130">Determine whether the rule support exclusions.</span></span> <span data-ttu-id="ec66d-131">Για λεπτομέρειες, ανατρέξτε στο [θέμα Κανόνες μείωσης επιφάνειας επίθεσης.](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)</span><span class="sxs-lookup"><span data-stu-id="ec66d-131">For details, see [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

1. <span data-ttu-id="ec66d-132">Εξετάστε τις εξαιρέσεις που εφαρμόστηκαν και επαληθεύστε με τα δεδομένα συμβάντος για λάθη ή εσφαλμένους χαρακτήρες μπαλαντέρ.</span><span class="sxs-lookup"><span data-stu-id="ec66d-132">Review the exclusions applied and verify with the event data for typos or misinterpreted wildcards.</span></span> <span data-ttu-id="ec66d-133">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Υποστηριζόμενοι τύποι αποκλεισμού](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span><span class="sxs-lookup"><span data-stu-id="ec66d-133">For more info, see [Supported exclusion types](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span></span>

1. <span data-ttu-id="ec66d-134">Εάν η επίδραση του κανόνα είναι πολύ υψηλή, εξετάστε το ενδεχόμενο να μετακινήσετε τον κανόνα (πίσω) σε λειτουργία ελέγχου για να εκτελέσετε περαιτέρω επικύρωση.</span><span class="sxs-lookup"><span data-stu-id="ec66d-134">if the impact of the rule it too high, consider moving the rule (back) to Audit mode to perform further validation.</span></span> <span data-ttu-id="ec66d-135">Για λεπτομέρειες, ανατρέξτε [στο θέμα Έλεγχος του τρόπου λειτουργίας των δυνατοτήτων του Microsoft Defender για τελικά σημεία σε λειτουργία ελέγχου.](/microsoft-365/security/defender-endpoint/audit-windows-defender)</span><span class="sxs-lookup"><span data-stu-id="ec66d-135">For details, see [Test how Microsoft Defender for Endpoint features work in audit mode](/microsoft-365/security/defender-endpoint/audit-windows-defender).</span></span>

1. <span data-ttu-id="ec66d-136">Συλλέξτε δεδομένα υποστήριξης για να ανοίξετε μια υπόθεση υποστήριξης χρησιμοποιώντας αυτή την εντολή:</span><span class="sxs-lookup"><span data-stu-id="ec66d-136">Collect support data to open a support case by using this command:</span></span>
    
   <span data-ttu-id="ec66d-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span><span class="sxs-lookup"><span data-stu-id="ec66d-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span></span>

    <span data-ttu-id="ec66d-138">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα Θέματα σχετικά με τους υπολογιστές με [πίνακες στο Microsoft Defender για τελικά σημεία.](issues-with-onboarding-machines.md)</span><span class="sxs-lookup"><span data-stu-id="ec66d-138">For more information, see [Issues with onboarding machines to Microsoft Defender for Endpoints](issues-with-onboarding-machines.md).</span></span>
