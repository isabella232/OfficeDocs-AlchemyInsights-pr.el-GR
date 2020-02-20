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
ms.openlocfilehash: 587a05cccbc71a970d4bd7723bff0df0c3b64ccc
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158561"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="ac87d-102">Δεν είναι δυνατός ο ορισμός ή η προβολή της πολιτικής AllowSelfServicePurchase</span><span class="sxs-lookup"><span data-stu-id="ac87d-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="ac87d-103">Όταν επιχειρείτε να ορίσετε ή να προβάλετε την πολιτική AllowSelfServicePurchase, λαμβάνετε το ακόλουθο μήνυμα λάθους:</span><span class="sxs-lookup"><span data-stu-id="ac87d-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="ac87d-104">*HandleError: απέτυχε η ανάκτηση της πολιτικής προϊόντος με PolicyId ' AllowSelfServicePurchase ', μήνυμα-η υποκείμενη σύνδεση έκλεισε: Παρουσιάστηκε ένα μη αναμενόμενο σφάλμα σε μια αποστολή.*</span><span class="sxs-lookup"><span data-stu-id="ac87d-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="ac87d-105">Αυτό μπορεί να οφείλεται σε παλαιότερη έκδοση της ασφάλειας επιπέδου μεταφοράς (TLS).</span><span class="sxs-lookup"><span data-stu-id="ac87d-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="ac87d-106">Για να συνδέσετε την υπηρεσία MSCommerce, πρέπει να χρησιμοποιήσετε το TLS 1,2 ή μεγαλύτερο.</span><span class="sxs-lookup"><span data-stu-id="ac87d-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="ac87d-107">Δοκιμάστε τα ακόλουθα βήματα για να ενεργοποιήσετε/ορίσετε το πρωτόκολλο TLS σε 1,2, επιβεβαιώστε και προσπαθήστε ξανά.</span><span class="sxs-lookup"><span data-stu-id="ac87d-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="ac87d-108">Στη γραμμή εντολών PowerShell (PS C:\) πληκτρολογήστε την ακόλουθη εντολή για να ορίσετε το πρωτόκολλο TLS στην έκδοση 1,2:</span><span class="sxs-lookup"><span data-stu-id="ac87d-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="ac87d-109">Επαληθεύστε τα πρωτόκολλα TLS που χρησιμοποιούνται, με την ακόλουθη εντολή:</span><span class="sxs-lookup"><span data-stu-id="ac87d-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="ac87d-110">Επαναλάβετε τις εντολές "λάβετε" ή "ενημέρωση", όπως απαιτείται.</span><span class="sxs-lookup"><span data-stu-id="ac87d-110">Retry the Get or Update commands as needed.</span></span>

