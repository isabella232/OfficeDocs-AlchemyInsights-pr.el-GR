---
title: DataProtection-BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: c23a2a2bde240900119382a9c1185a6e02520149
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908710"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="a6c43-102">Ενεργοποίηση της κρυπτογράφησης BitLocker με το Intune</span><span class="sxs-lookup"><span data-stu-id="a6c43-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="a6c43-103">Η πολιτική προστασίας Intune Endpoint μπορεί να χρησιμοποιηθεί για τη ρύθμιση των παραμέτρων κρυπτογράφησης BitLocker για συσκευές Windows.</span><span class="sxs-lookup"><span data-stu-id="a6c43-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="a6c43-104">Για περισσότερες πληροφορίες, ανατρέξτε [στις ρυθμίσεις των Windows 10 (και νεότερες) για την προστασία συσκευών που χρησιμοποιούν Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="a6c43-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="a6c43-105">Θα πρέπει να γνωρίζετε ότι πολλές νεότερες συσκευές που εκτελούν Windows 10 υποστηρίζουν την αυτόματη κρυπτογράφηση BitLocker, η οποία ενεργοποιείται χωρίς την εφαρμογή της πολιτικής της ΤΚ.</span><span class="sxs-lookup"><span data-stu-id="a6c43-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="a6c43-106">Αυτό μπορεί να επηρεάσει την εφαρμογή της πολιτικής, εάν έχουν ρυθμιστεί μη προεπιλεγμένες ρυθμίσεις.</span><span class="sxs-lookup"><span data-stu-id="a6c43-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="a6c43-107">Για περισσότερες λεπτομέρειες, ανατρέξτε στις παρακάτω Συνήθεις ερωτήσεις.</span><span class="sxs-lookup"><span data-stu-id="a6c43-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="a6c43-108">Για πληροφορίες σχετικά με την αντιμετώπιση προβλημάτων BitLocker, ανατρέξτε [στο θέμα Αντιμετώπιση προβλημάτων πολιτικών BitLocker στο Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="a6c43-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="a6c43-109">**Συνήθεις ερωτήσεις**</span><span class="sxs-lookup"><span data-stu-id="a6c43-109">**FAQ**</span></span>

 <span data-ttu-id="a6c43-110">Ε: Ποιες εκδόσεις των Windows υποστηρίζουν κρυπτογράφηση συσκευών χρησιμοποιώντας την πολιτική Endpoint Protection;</span><span class="sxs-lookup"><span data-stu-id="a6c43-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
 <span data-ttu-id="a6c43-111">A: οι ρυθμίσεις στην πολιτική προστασίας Intune Endpoint υλοποιούνται χρησιμοποιώντας το [BitLocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span><span class="sxs-lookup"><span data-stu-id="a6c43-111">A: The settings in Intune Endpoint Protection Policy  are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="a6c43-112">Δεν υποστηρίζουν όλες οι εκδόσεις ή οι εκδόσεις των Windows το BitLocker CSP.</span><span class="sxs-lookup"><span data-stu-id="a6c43-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>
      <span data-ttu-id="a6c43-113">Αυτή τη στιγμή, υποστηρίζονται οι ακόλουθες εκδόσεις των Windows: επιχείρηση, εκπαίδευση, κινητές συσκευές, κινητή επιχείρηση και επαγγελματική (build 1809 και νεότερα).</span><span class="sxs-lookup"><span data-stu-id="a6c43-113">At this time, the following Windows editions are supported: Enterprise, Education, Mobile, Mobile Enterprise, and Professional (build 1809 and later).</span></span>
 
<span data-ttu-id="a6c43-114">Ε: Εάν μια συσκευή είναι ήδη κρυπτογραφημένη με το BitLocker χρησιμοποιώντας τις προεπιλεγμένες ρυθμίσεις λειτουργικού συστήματος για τη μέθοδο κρυπτογράφησης και την ισχύ κρυπτογράφησης (XTS-AES-128), η εφαρμογή μιας πολιτικής με διαφορετικές ρυθμίσεις θα ενεργοποιήσει αυτόματα την επανακρυπτογράφηση της μονάδας δίσκου με τις νέες ρυθμίσεις;</span><span class="sxs-lookup"><span data-stu-id="a6c43-114">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="a6c43-115">Α: Όχι.</span><span class="sxs-lookup"><span data-stu-id="a6c43-115">A: No.</span></span> <span data-ttu-id="a6c43-116">Για να εφαρμόσετε τις νέες ρυθμίσεις κρυπτογράφησης, η μονάδα δίσκου πρέπει πρώτα να αποκρυπτογραφηθεί.</span><span class="sxs-lookup"><span data-stu-id="a6c43-116">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="a6c43-117">**Σημείωση:** Για συσκευές που εγγράφονται με τον αυτόματο πιλότο, η αυτόματη κρυπτογράφηση που θα προκύψει κατά τη διάρκεια του OOBE δεν ενεργοποιείται μέχρι να αξιολογηθεί η πολιτική Intune, η οποία επιτρέπει τη χρήση των ρυθμίσεων που βασίζονται στην πολιτική στη θέση των προεπιλογών λειτουργικού συστήματος.</span><span class="sxs-lookup"><span data-stu-id="a6c43-117">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="a6c43-118">Ε: Εάν μια συσκευή είναι κρυπτογραφημένη ως αποτέλεσμα της εφαρμογής της πολιτικής Intune, θα αποκρυπτογραφηθεί όταν καταργηθεί αυτή η πολιτική;</span><span class="sxs-lookup"><span data-stu-id="a6c43-118">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="a6c43-119">A: η κατάργηση της πολιτικής που σχετίζεται με την κρυπτογράφηση δεν έχει ως αποτέλεσμα την αποκρυπτογράφηση των μονάδων δίσκου που έχουν ρυθμιστεί.</span><span class="sxs-lookup"><span data-stu-id="a6c43-119">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="a6c43-120">Ε: Γιατί η πολιτική συμμόρφωσης Intune δείχνει ότι η συσκευή μου δεν έχει ενεργοποιημένο το BitLocker, ακόμα κι αν είναι;</span><span class="sxs-lookup"><span data-stu-id="a6c43-120">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="a6c43-121">A: η ρύθμιση "ενεργοποιημένη BitLocker" στην πολιτική συμμόρφωσης Intune χρησιμοποιεί τον υπολογιστή-πελάτη βεβαίωση εύρυθμης λειτουργίας συσκευών των Windows.</span><span class="sxs-lookup"><span data-stu-id="a6c43-121">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="a6c43-122">Αυτό το πρόγραμμα-πελάτης μετρά μόνο την κατάσταση της συσκευής κατά το χρόνο εκκίνησης.</span><span class="sxs-lookup"><span data-stu-id="a6c43-122">This client only measures device state at boot time.</span></span> <span data-ttu-id="a6c43-123">Επομένως, εάν δεν έχει γίνει επανεκκίνηση μιας συσκευής από την ολοκλήρωση της κρυπτογράφησης BitLocker, η υπηρεσία προγράμματος-πελάτη</span><span class="sxs-lookup"><span data-stu-id="a6c43-123">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 