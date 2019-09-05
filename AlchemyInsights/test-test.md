---
title: Όροι που λείπουν από το SharePoint Online αποθήκευσης όρων
ms.author: pebaum
author: Techwriter40
ms.date: 10/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 0f9efe980987c9ffc64fcf9d5d72a67f0a622867
ms.sourcegitcommit: 23772ebd25a86a879ced40b10566a35e76a79eb5
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/05/2019
ms.locfileid: "36762061"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="95f61-102">Ενεργοποίηση της κρυπτογράφησης BitLocker με το Intune</span><span class="sxs-lookup"><span data-stu-id="95f61-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="95f61-103">Η πολιτική προστασίας Intune Endpoint μπορεί να χρησιμοποιηθεί για τη ρύθμιση των ρυθμίσεων κρυπτογράφησης για συσκευές Windows, όπως περιγράφεται σε: Windows10 (και νεότερες) ρυθμίσεις για την προστασία συσκευών που χρησιμοποιούν Intune</span><span class="sxs-lookup"><span data-stu-id="95f61-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="95f61-104">Θα πρέπει να γνωρίζετε ότι πολλές νεότερες συσκευές που εκτελούν Windows 10 υποστηρίζουν την αυτόματη κρυπτογράφηση BitLocker, η οποία ενεργοποιείται χωρίς την εφαρμογή της πολιτικής της ΤΚ.</span><span class="sxs-lookup"><span data-stu-id="95f61-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="95f61-105">Αυτό μπορεί να επηρεάσει την εφαρμογή της πολιτικής, εάν έχουν ρυθμιστεί μη προεπιλεγμένες ρυθμίσεις.</span><span class="sxs-lookup"><span data-stu-id="95f61-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="95f61-106">Δείτε συνήθεις ερωτήσεις για περισσότερες λεπτομέρειες.</span><span class="sxs-lookup"><span data-stu-id="95f61-106">See FAQ for more detail.</span></span>


<span data-ttu-id="95f61-107">Συχνές  ερωτήσεις Q: Ποιες εκδόσεις των Windows υποστηρίζουν κρυπτογράφηση συσκευών χρησιμοποιώντας την πολιτική Endpoint Protection;</span><span class="sxs-lookup"><span data-stu-id="95f61-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="95f61-108"> A: οι ρυθμίσεις στο Intune Endpoint Protection πολιτική υλοποιούνται χρησιμοποιώντας το BitLocker CSP.</span><span class="sxs-lookup"><span data-stu-id="95f61-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="95f61-109">Δεν υποστηρίζουν όλες οι εκδόσεις ή εκδόσεις των Windows το BitLocker CSP. 
     </span><span class="sxs-lookup"><span data-stu-id="95f61-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="95f61-110">Αυτή τη στιγμή εκδόσεις των Windows: Enterprise? Η εκπαίδευση, το κινητό, η κινητή επιχείρηση και ο επαγγελματίας (από το build 1809 και μετά) υποστηρίζονται.</span><span class="sxs-lookup"><span data-stu-id="95f61-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="95f61-111">Ε: Εάν μια συσκευή είναι ήδη κρυπτογραφημένη με το BitLocker χρησιμοποιώντας τις προεπιλεγμένες ρυθμίσεις λειτουργικού συστήματος για τη μέθοδο κρυπτογράφησης και την ισχύ κρυπτογράφησης (XTS-AES-128), η εφαρμογή μιας πολιτικής με διαφορετικές ρυθμίσεις θα ενεργοποιήσει αυτόματα την επανακρυπτογράφηση της μονάδας δίσκου με τις νέες ρυθμίσεις;</span><span class="sxs-lookup"><span data-stu-id="95f61-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="95f61-112">Α: Όχι.</span><span class="sxs-lookup"><span data-stu-id="95f61-112">A: No.</span></span> <span data-ttu-id="95f61-113">Για να εφαρμόσετε τις νέες ρυθμίσεις κρυπτογράφησης, η μονάδα δίσκου πρέπει πρώτα να αποκρυπτογραφηθεί.</span><span class="sxs-lookup"><span data-stu-id="95f61-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="95f61-114">Σημείωση για συσκευές που εγγράφονται με τον αυτόματο πιλότο η αυτόματη κρυπτογράφηση που θα προκύψει κατά τη διάρκεια του OOBE δεν ενεργοποιείται μέχρι να αξιολογηθεί η πολιτική Intune, η οποία επιτρέπει τη χρήση των ρυθμίσεων που βασίζονται στην πολιτική στη θέση των προεπιλογών λειτουργικού συστήματος</span><span class="sxs-lookup"><span data-stu-id="95f61-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="95f61-115">Q Εάν μια συσκευή είναι κρυπτογραφημένη ως αποτέλεσμα της εφαρμογής της πολιτικής Intune θα αποκρυπτογραφηθεί όταν καταργηθεί αυτή η πολιτική;</span><span class="sxs-lookup"><span data-stu-id="95f61-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="95f61-116">A: η κατάργηση της πολιτικής που σχετίζεται με την κρυπτογράφηση δεν έχει ως αποτέλεσμα την αποκρυπτογράφηση των μονάδων δίσκου που έχουν ρυθμιστεί.</span><span class="sxs-lookup"><span data-stu-id="95f61-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="95f61-117">Ε: Γιατί η πολιτική συμμόρφωσης Intune δείχνει ότι η συσκευή μου δεν έχει "ενεργοποιημένο BitLocker" αλλά είναι;</span><span class="sxs-lookup"><span data-stu-id="95f61-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="95f61-118">A: η ρύθμιση "ενεργοποιημένη BitLocker" στην πολιτική Intune συμμόρφωσης χρησιμοποιεί το πρόγραμμα-πελάτη πιστοποίησης εύρυθμης λειτουργίας συσκευών των Windows.</span><span class="sxs-lookup"><span data-stu-id="95f61-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="95f61-119">Αυτό το πρόγραμμα-πελάτης μετρά μόνο την κατάσταση της συσκευής κατά το χρόνο εκκίνησης.</span><span class="sxs-lookup"><span data-stu-id="95f61-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="95f61-120">Επομένως, εάν δεν έγινε επανεκκίνηση μιας συσκευής από την ολοκλήρωση της κρυπτογράφησης BitLocker, η υπηρεσία πελάτη</span><span class="sxs-lookup"><span data-stu-id="95f61-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>