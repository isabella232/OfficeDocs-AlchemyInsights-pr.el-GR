---
title: DataProtection-BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: ab28162fcdf0a37060be3bdf15a78aceca7a48b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731239"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="ea452-102">Ενεργοποίηση της κρυπτογράφησης BitLocker με το Intune</span><span class="sxs-lookup"><span data-stu-id="ea452-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="ea452-103">Η πολιτική προστασίας απόληξης του Intune μπορεί να χρησιμοποιηθεί για τη ρύθμιση των παραμέτρων κρυπτογράφησης BitLocker για συσκευές Windows.</span><span class="sxs-lookup"><span data-stu-id="ea452-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="ea452-104">Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα ρυθμίσεις των Windows 10 (και νεότερες εκδόσεις) για την προστασία των συσκευών με χρήση του Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="ea452-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="ea452-105">Θα πρέπει να γνωρίζετε ότι πολλές νεότερες συσκευές που χρησιμοποιούν Windows 10 υποστηρίζουν την αυτόματη κρυπτογράφηση BitLocker, η οποία ενεργοποιείται χωρίς την εφαρμογή της πολιτικής MDM.</span><span class="sxs-lookup"><span data-stu-id="ea452-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="ea452-106">Αυτό μπορεί να επηρεάσει την εφαρμογή της πολιτικής, εάν έχουν ρυθμιστεί μη προεπιλεγμένες ρυθμίσεις.</span><span class="sxs-lookup"><span data-stu-id="ea452-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="ea452-107">Ανατρέξτε στις παρακάτω Συνήθεις ερωτήσεις για περισσότερες λεπτομέρειες.</span><span class="sxs-lookup"><span data-stu-id="ea452-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="ea452-108">Για πληροφορίες σχετικά με την αντιμετώπιση προβλημάτων του BitLocker, ανατρέξτε [στο θέμα Αντιμετώπιση προβλημάτων με τις πολιτικές BitLocker στο Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="ea452-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="ea452-109">**ΣΥΝΗΘΕΙΣ ΕΡΩΤΉΣΕΙΣ**</span><span class="sxs-lookup"><span data-stu-id="ea452-109">**FAQ**</span></span>

 <span data-ttu-id="ea452-110">Ε: Ποιες εκδόσεις του Windows υποστηρίζουν την κρυπτογράφηση συσκευών με χρήση της πολιτικής προστασίας τελικού σημείου;</span><span class="sxs-lookup"><span data-stu-id="ea452-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
 <span data-ttu-id="ea452-111">Α: οι ρυθμίσεις στην πολιτική προστασίας τελικού σημείου του Intune υλοποιούνται με χρήση της [CSP CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span><span class="sxs-lookup"><span data-stu-id="ea452-111">A: The settings in Intune Endpoint Protection Policy  are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="ea452-112">Η υπηρεσία CSP BitLocker δεν υποστηρίζει όλες τις εκδόσεις ή τις εκδόσεις των Windows.</span><span class="sxs-lookup"><span data-stu-id="ea452-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>
      <span data-ttu-id="ea452-113">Προς το παρόν, υποστηρίζονται οι ακόλουθες εκδόσεις των Windows: Enterprise, Education, Mobile, Mobile Enterprise και Professional (δομή 1809 και νεότερες εκδόσεις).</span><span class="sxs-lookup"><span data-stu-id="ea452-113">At this time, the following Windows editions are supported: Enterprise, Education, Mobile, Mobile Enterprise, and Professional (build 1809 and later).</span></span>
 
<span data-ttu-id="ea452-114">Ε: Εάν μια συσκευή είναι ήδη κρυπτογραφημένη με το BitLocker χρησιμοποιώντας τις προεπιλεγμένες ρυθμίσεις του λειτουργικού συστήματος για τη μέθοδο κρυπτογράφησης και τη δύναμη κρυπτογράφησης (XTS-AES-128), η εφαρμογή μιας πολιτικής με διαφορετικές ρυθμίσεις ενεργοποιεί αυτόματα την εκ νέου κρυπτογράφηση της μονάδας δίσκου με τις νέες ρυθμίσεις;</span><span class="sxs-lookup"><span data-stu-id="ea452-114">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="ea452-115">Α: Όχι.</span><span class="sxs-lookup"><span data-stu-id="ea452-115">A: No.</span></span> <span data-ttu-id="ea452-116">Για να εφαρμόσετε τις νέες ρυθμίσεις κρυπτογράφησης, η μονάδα δίσκου πρέπει πρώτα να αποκρυπτογραφηθεί.</span><span class="sxs-lookup"><span data-stu-id="ea452-116">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="ea452-117">**Σημείωση:** Για τις συσκευές που είναι εγγεγραμμένες με τον αυτόματο πιλότο, η αυτόματη κρυπτογράφηση που θα προκύψει κατά τη φάση OOBE δεν ενεργοποιείται μέχρι την αξιολόγηση της πολιτικής Intune, η οποία επιτρέπει τη χρήση των ρυθμίσεων που βασίζονται σε πολιτική στη θέση των προεπιλογών του λειτουργικού συστήματος.</span><span class="sxs-lookup"><span data-stu-id="ea452-117">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="ea452-118">Ε: Εάν μια συσκευή είναι κρυπτογραφημένη ως αποτέλεσμα της εφαρμογής της πολιτικής Intune, θα αποκρυπτογραφηθεί όταν καταργηθεί αυτή η πολιτική;</span><span class="sxs-lookup"><span data-stu-id="ea452-118">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="ea452-119">Α: η κατάργηση της πολιτικής που σχετίζεται με την κρυπτογράφηση δεν έχει ως αποτέλεσμα την αποκρυπτογράφηση των μονάδων δίσκου που έχουν ρυθμιστεί.</span><span class="sxs-lookup"><span data-stu-id="ea452-119">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="ea452-120">Ε: Γιατί η πολιτική συμμόρφωσης του Intune δείχνει ότι η συσκευή μου δεν έχει ενεργοποιημένο το BitLocker, παρόλο που είναι;</span><span class="sxs-lookup"><span data-stu-id="ea452-120">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="ea452-121">Α: η ρύθμιση "Enabled BitLocker" στην πολιτική συμμόρφωσης του Intune χρησιμοποιεί το πρόγραμμα-πελάτη για τη βεβαίωση εύρυθμης λειτουργίας συσκευών των Windows (DHA).</span><span class="sxs-lookup"><span data-stu-id="ea452-121">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="ea452-122">Αυτό το πρόγραμμα-πελάτης μετράει μόνο την κατάσταση συσκευής κατά την εκκίνηση.</span><span class="sxs-lookup"><span data-stu-id="ea452-122">This client only measures device state at boot time.</span></span> <span data-ttu-id="ea452-123">Επομένως, εάν δεν έχει γίνει επανεκκίνηση μιας συσκευής από την ολοκλήρωση της κρυπτογράφησης BitLocker, η υπηρεσία προγράμματος-πελάτη DHA δεν θα αναφέρει ότι το BitLocker είναι ενεργό.</span><span class="sxs-lookup"><span data-stu-id="ea452-123">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 