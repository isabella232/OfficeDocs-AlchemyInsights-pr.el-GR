---
title: Λείπουν όροι από το χώρο αποθήκευσης όρων του SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 06711c289365c0fcdf71cf9cccf3cfc53511495a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750451"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="633f7-102">Ενεργοποίηση της κρυπτογράφησης BitLocker με το Intune</span><span class="sxs-lookup"><span data-stu-id="633f7-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="633f7-103">Η πολιτική προστασίας απόληξης του Intune μπορεί να χρησιμοποιηθεί για τη ρύθμιση παραμέτρων των ρυθμίσεων κρυπτογράφησης του Boitlocker για συσκευές Windows, όπως περιγράφεται στις: Windows10 (και νεότερες εκδόσεις) για την προστασία των συσκευών με χρήση του Intune</span><span class="sxs-lookup"><span data-stu-id="633f7-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="633f7-104">Θα πρέπει να γνωρίζετε ότι πολλές νεότερες συσκευές που χρησιμοποιούν Windows 10 υποστηρίζουν την αυτόματη κρυπτογράφηση BitLocker, η οποία ενεργοποιείται χωρίς την εφαρμογή της πολιτικής MDM.</span><span class="sxs-lookup"><span data-stu-id="633f7-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="633f7-105">Αυτό μπορεί να επηρεάσει την εφαρμογή της πολιτικής, εάν δεν ρυθμιστούν οι προεπιλεγμένες ρυθμίσεις.</span><span class="sxs-lookup"><span data-stu-id="633f7-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="633f7-106">Ανατρέξτε στο θέμα Συνήθεις ερωτήσεις για περισσότερες λεπτομέρειες.</span><span class="sxs-lookup"><span data-stu-id="633f7-106">See FAQ for more detail.</span></span>


<span data-ttu-id="633f7-107">Συνήθεις ερωτήσεις   : Ποιες εκδόσεις των Windows υποστηρίζουν την κρυπτογράφηση συσκευών με χρήση της πολιτικής προστασίας τελικού σημείου;</span><span class="sxs-lookup"><span data-stu-id="633f7-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="633f7-108"> Α: οι ρυθμίσεις στην πολιτική προστασίας τελικού σημείου του Intune υλοποιούνται με χρήση της CSP CSP.</span><span class="sxs-lookup"><span data-stu-id="633f7-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="633f7-109">Η υπηρεσία CSP BitLocker δεν υποστηρίζει όλες τις εκδόσεις ούτε τις εκδόσεις των Windows. 
     </span><span class="sxs-lookup"><span data-stu-id="633f7-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="633f7-110">Αυτήν τη στιγμή, οι εκδόσεις των Windows: Enterprise; Υποστηρίζονται η εκπαίδευση, το κινητό, η κινητή επιχείρηση και ο επαγγελματίας (από τη δομή 1809 και μετά).</span><span class="sxs-lookup"><span data-stu-id="633f7-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="633f7-111">Ε: Εάν μια συσκευή είναι ήδη κρυπτογραφημένη με το BitLocker χρησιμοποιώντας τις προεπιλεγμένες ρυθμίσεις του λειτουργικού συστήματος για τη μέθοδο κρυπτογράφησης και τη δύναμη κρυπτογράφησης (XTS-AES-128), η εφαρμογή μιας πολιτικής με διαφορετικές ρυθμίσεις ενεργοποιεί αυτόματα την εκ νέου κρυπτογράφηση της μονάδας δίσκου με τις νέες ρυθμίσεις;</span><span class="sxs-lookup"><span data-stu-id="633f7-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="633f7-112">Α: Όχι.</span><span class="sxs-lookup"><span data-stu-id="633f7-112">A: No.</span></span> <span data-ttu-id="633f7-113">Για να εφαρμόσετε τις νέες ρυθμίσεις κρυπτογράφησης, πρέπει πρώτα να αποκρυπτογραφηθεί η μονάδα δίσκου.</span><span class="sxs-lookup"><span data-stu-id="633f7-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="633f7-114">Σημείωση για τις συσκευές που εγγράφονται με αυτόματο πιλότο η αυτόματη κρυπτογράφηση που θα προκύψει κατά τη φάση OOBE δεν ενεργοποιείται μέχρι την αξιολόγηση της πολιτικής Intune, η οποία επιτρέπει τη χρήση των ρυθμίσεων που βασίζονται σε πολιτική στη θέση των προεπιλογών του λειτουργικού συστήματος</span><span class="sxs-lookup"><span data-stu-id="633f7-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="633f7-115">Q Εάν μια συσκευή είναι κρυπτογραφημένη ως αποτέλεσμα της εφαρμογής της πολιτικής Intune θα αποκρυπτογραφηθεί όταν καταργηθεί αυτή η πολιτική;</span><span class="sxs-lookup"><span data-stu-id="633f7-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="633f7-116">Α: η κατάργηση της πολιτικής που σχετίζεται με την κρυπτογράφηση δεν έχει ως αποτέλεσμα την αποκρυπτογράφηση των μονάδων δίσκου που έχουν ρυθμιστεί.</span><span class="sxs-lookup"><span data-stu-id="633f7-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="633f7-117">Ε: Γιατί η πολιτική συμμόρφωσης του Intune δείχνει ότι η συσκευή μου δεν έχει "ενεργοποιημένο BitLocker", αλλά είναι;</span><span class="sxs-lookup"><span data-stu-id="633f7-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="633f7-118">Α: η ρύθμιση "με δυνατότητα BitLocker" στην πολιτική συμμόρφωσης του Intune χρησιμοποιεί το πρόγραμμα-πελάτη για τη βεβαίωση εύρυθμης λειτουργίας συσκευών των Windows (DHA).</span><span class="sxs-lookup"><span data-stu-id="633f7-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="633f7-119">Αυτό το πρόγραμμα-πελάτης μετράει μόνο την κατάσταση συσκευής κατά την εκκίνηση.</span><span class="sxs-lookup"><span data-stu-id="633f7-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="633f7-120">Επομένως, εάν δεν έχει γίνει επανεκκίνηση μιας συσκευής μετά την ολοκλήρωση της κρυπτογράφησης BitLocker, η υπηρεσία προγράμματος-πελάτη DHA δεν θα αναφέρει ότι το BitLocker είναι ενεργό.</span><span class="sxs-lookup"><span data-stu-id="633f7-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>