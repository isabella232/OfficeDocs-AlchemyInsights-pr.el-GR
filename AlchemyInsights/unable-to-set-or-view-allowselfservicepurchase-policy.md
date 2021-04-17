---
title: Δεν είναι δυνατός ο ορισμός ή η προβολή της πολιτικής AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 8dac2bdc20905cf37fc30317d9b371bfd755f452
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826091"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="60279-102">Δεν είναι δυνατός ο ορισμός ή η προβολή της πολιτικής AllowSelfServicePurchase</span><span class="sxs-lookup"><span data-stu-id="60279-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="60279-103">Όταν προσπαθείτε να ορίσετε ή να προβάλετε την πολιτική AllowSelfServicePurchase, λαμβάνετε το ακόλουθο μήνυμα σφάλματος:</span><span class="sxs-lookup"><span data-stu-id="60279-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="60279-104">*HandleError : Απέτυχε η ανάκτηση πολιτικής προϊόντος με το PolicyId "AllowSelfServicePurchase", ErrorMessage - Η υποκείμενη σύνδεση έκλεισε: Παρουσιάστηκε μη αναμενόμενο σφάλμα κατά την αποστολή.*</span><span class="sxs-lookup"><span data-stu-id="60279-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="60279-105">Αυτό μπορεί να οφείλεται σε μια παλαιότερη έκδοση του Transport Layer Security (TLS).</span><span class="sxs-lookup"><span data-stu-id="60279-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="60279-106">Για να συνδέσετε την υπηρεσία MSCommerce, πρέπει να χρησιμοποιήσετε TLS 1.2 ή μεγαλύτερο.</span><span class="sxs-lookup"><span data-stu-id="60279-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="60279-107">Δοκιμάστε τα παρακάτω βήματα για να ενεργοποιήσετε/ορίσετε το πρωτόκολλο TLS σε 1,2, να επαληθεύσετε και να επαναλάβετε την προσπάθεια.</span><span class="sxs-lookup"><span data-stu-id="60279-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="60279-108">Στη γραμμή εντολών του PowerShell (PS C: πληκτρολογήστε την ακόλουθη εντολή για να \) ορίσετε το πρωτόκολλο TLS στην έκδοση 1.2:</span><span class="sxs-lookup"><span data-stu-id="60279-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="60279-109">Επαληθεύστε τα πρωτόκολλα TLS που χρησιμοποιούνται, με την ακόλουθη εντολή:</span><span class="sxs-lookup"><span data-stu-id="60279-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="60279-110">Επαναλάβετε τις εντολές "Λήψη" ή "Ενημέρωση", όπως απαιτείται.</span><span class="sxs-lookup"><span data-stu-id="60279-110">Retry the Get or Update commands as needed.</span></span>

