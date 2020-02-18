---
title: Δεν είναι δυνατός ο ορισμός ή η προβολή της πολιτικής AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: a9b6e36e8034e71b3e72c49e3cc68a126ef97aca
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091706"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="9e7c2-102">Δεν είναι δυνατός ο ορισμός ή η προβολή της πολιτικής AllowSelfServicePurchase</span><span class="sxs-lookup"><span data-stu-id="9e7c2-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="9e7c2-103">Όταν επιχειρείτε να ορίσετε ή να προβάλετε την πολιτική AllowSelfServicePurchase, λαμβάνετε το ακόλουθο μήνυμα λάθους:</span><span class="sxs-lookup"><span data-stu-id="9e7c2-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="9e7c2-104">*HandleError: απέτυχε η ανάκτηση της πολιτικής προϊόντος με PolicyId ' AllowSelfServicePurchase ', μήνυμα-η υποκείμενη σύνδεση έκλεισε: Παρουσιάστηκε ένα μη αναμενόμενο σφάλμα σε μια αποστολή.*</span><span class="sxs-lookup"><span data-stu-id="9e7c2-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="9e7c2-105">Αυτό μπορεί να οφείλεται σε παλαιότερη έκδοση της ασφάλειας επιπέδου μεταφοράς (TLS).</span><span class="sxs-lookup"><span data-stu-id="9e7c2-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="9e7c2-106">Για να συνδέσετε την υπηρεσία MSCommerce, πρέπει να χρησιμοποιήσετε το TLS 1,2 ή μεγαλύτερο.</span><span class="sxs-lookup"><span data-stu-id="9e7c2-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="9e7c2-107">Δοκιμάστε τα ακόλουθα βήματα για να ενεργοποιήσετε/ορίσετε το πρωτόκολλο TLS σε 1,2, επιβεβαιώστε και προσπαθήστε ξανά.</span><span class="sxs-lookup"><span data-stu-id="9e7c2-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="9e7c2-108">Στη γραμμή εντολών PowerShell (PS C:\) πληκτρολογήστε την ακόλουθη εντολή για να ορίσετε το πρωτόκολλο TLS στην έκδοση 1,2:</span><span class="sxs-lookup"><span data-stu-id="9e7c2-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    <span data-ttu-id="9e7c2-109">\[NET. ServicePointManager]:: SecurityProtocol = \[NET. SecurityProtocolType]:: Tls12</span><span class="sxs-lookup"><span data-stu-id="9e7c2-109">\[Net.ServicePointManager]::SecurityProtocol = \[Net.SecurityProtocolType]::Tls12</span></span>

2. <span data-ttu-id="9e7c2-110">Επαληθεύστε τα πρωτόκολλα TLS που χρησιμοποιούνται, με την ακόλουθη εντολή:</span><span class="sxs-lookup"><span data-stu-id="9e7c2-110">Verify the TLS protocol(s) in use, with the following command:</span></span>

    <span data-ttu-id="9e7c2-111">\[NET. ServicePointManager]:: SecurityProtocol</span><span class="sxs-lookup"><span data-stu-id="9e7c2-111">\[Net.ServicePointManager]::SecurityProtocol</span></span> 

3. <span data-ttu-id="9e7c2-112">Επαναλάβετε τις εντολές "λάβετε" ή "ενημέρωση", όπως απαιτείται.</span><span class="sxs-lookup"><span data-stu-id="9e7c2-112">Retry the Get or Update commands as needed.</span></span>

