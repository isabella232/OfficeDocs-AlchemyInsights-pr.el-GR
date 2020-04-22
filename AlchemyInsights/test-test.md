---
title: Όροι που λείπουν από το SharePoint Online Term Store
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 54ac2dbc1f45f88541c2338f3b55a777b4b57123
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766853"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="e8362-102">Ενεργοποίηση κρυπτογράφησης Bitlocker με το Intune</span><span class="sxs-lookup"><span data-stu-id="e8362-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="e8362-103">Η πολιτική προστασίας τελικού σημείου Intune μπορεί να χρησιμοποιηθεί για τη ρύθμιση παραμέτρων κρυπτογράφησης Boitlocker για συσκευές Windows, όπως περιγράφεται στο : Ρυθμίσεις Windows10 (και νεότερες εκδόσεις) για την προστασία συσκευών που χρησιμοποιούν το Intune</span><span class="sxs-lookup"><span data-stu-id="e8362-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="e8362-104">Θα πρέπει να γνωρίζετε ότι πολλές νεότερες συσκευές που εκτελούν Windows 10 υποστηρίζουν αυτόματη κρυπτογράφηση bitlocker, η οποία ενεργοποιείται χωρίς την εφαρμογή της πολιτικής MDM.</span><span class="sxs-lookup"><span data-stu-id="e8362-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="e8362-105">Αυτό μπορεί να επηρεάσει την εφαρμογή της πολιτικής, εάν δεν έχουν ρυθμιστεί οι προεπιλεγμένες ρυθμίσεις.</span><span class="sxs-lookup"><span data-stu-id="e8362-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="e8362-106">Ανατρέξτε στις Συνήθεις ερωτήσεις για περισσότερες λεπτομέρειες.</span><span class="sxs-lookup"><span data-stu-id="e8362-106">See FAQ for more detail.</span></span>


<span data-ttu-id="e8362-107">Συχνές  ερωτήσεις Q: Ποιες εκδόσεις κρυπτογράφησης συσκευών υποστήριξης των Windows χρησιμοποιούν την Πολιτική προστασίας τελικού σημείου;</span><span class="sxs-lookup"><span data-stu-id="e8362-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="e8362-108"> A: Οι ρυθμίσεις στην Πολιτική προστασίας τελικού σημείου Intune υλοποιούνται χρησιμοποιώντας το CSP Bitlocker.</span><span class="sxs-lookup"><span data-stu-id="e8362-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="e8362-109">Δεν υποστηρίζουν όλες οι εκδόσεις ούτε οι εκδόσεις των Windows το CSP Bitlocker. 
     </span><span class="sxs-lookup"><span data-stu-id="e8362-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="e8362-110">Αυτή τη στιγμή εκδόσεις των Windows: Enterprise? Η εκπαίδευση, κινητός, κινητός επιχείρηση και επαγγελματικός (από την κατασκευή 1809 και μετά) υποστηρίζεται.</span><span class="sxs-lookup"><span data-stu-id="e8362-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="e8362-111">Ε: Εάν μια συσκευή είναι ήδη κρυπτογραφημένη με Το Bitlocker χρησιμοποιώντας τις προεπιλεγμένες ρυθμίσεις os για τη μέθοδο κρυπτογράφησης και την ισχύ κρυπτογράφησης (XTS-AES-128) θα εφαρμόσει μια πολιτική με διαφορετικές ρυθμίσεις ενεργοποιεί αυτόματα την εκ νέου κρυπτογράφηση της μονάδας δίσκου με τις νέες ρυθμίσεις;</span><span class="sxs-lookup"><span data-stu-id="e8362-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="e8362-112">Α: Όχι.</span><span class="sxs-lookup"><span data-stu-id="e8362-112">A: No.</span></span> <span data-ttu-id="e8362-113">Για να εφαρμοστούν οι νέες ρυθμίσεις κρυπτογράφησης, η μονάδα δίσκου πρέπει πρώτα να αποκρυπτογραφηθεί.</span><span class="sxs-lookup"><span data-stu-id="e8362-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="e8362-114">Σημείωση Για συσκευές που εγγράφονται με αυτόματο πιλότο, η αυτόματη κρυπτογράφηση που θα προκύψει κατά τη διάρκεια του OOBE δεν ενεργοποιείται μέχρι να αξιολογηθεί η πολιτική Intune, η οποία επιτρέπει τη χρήση των ρυθμίσεων βάσει πολιτικής στη θέση των προεπιλογών λειτουργικού συστήματος</span><span class="sxs-lookup"><span data-stu-id="e8362-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="e8362-115">Q Εάν μια συσκευή είναι κρυπτογραφημένη ως αποτέλεσμα της εφαρμογής της πολιτικής Intune, θα αποκρυπτογραφηθεί όταν καταργηθεί αυτή η πολιτική;</span><span class="sxs-lookup"><span data-stu-id="e8362-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="e8362-116">A: Η κατάργηση της πολιτικής που σχετίζεται με την κρυπτογράφηση ΔΕΝ έχει ως αποτέλεσμα την αποκρυπτογράφηση των μονάδων δίσκου που έχουν ρυθμιστεί.</span><span class="sxs-lookup"><span data-stu-id="e8362-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="e8362-117">Ε: Γιατί η πολιτική συμμόρφωσης intune δείχνει ότι η συσκευή μου δεν έχει "Bitlocker Enabled", αλλά είναι;</span><span class="sxs-lookup"><span data-stu-id="e8362-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="e8362-118">A: Η ρύθμιση "Bitlocker ενεργοποιημένη" στην πολιτική συμμόρφωσης intune χρησιμοποιεί το πρόγραμμα-πελάτη διαπιστώσεως εύρυθμης λειτουργίας συσκευής των Windows (DHA).</span><span class="sxs-lookup"><span data-stu-id="e8362-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="e8362-119">Αυτός ο υπολογιστής-πελάτης μετρά μόνο την κατάσταση της συσκευής κατά την εκκίνηση.</span><span class="sxs-lookup"><span data-stu-id="e8362-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="e8362-120">Έτσι, εάν δεν έχει γίνει επανεκκίνηση μιας συσκευής από την ολοκλήρωση της κρυπτογράφησης bitlocker, η υπηρεσία-πελάτης DHA δεν θα αναφέρει ότι το bitlocker είναι ενεργό.</span><span class="sxs-lookup"><span data-stu-id="e8362-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>