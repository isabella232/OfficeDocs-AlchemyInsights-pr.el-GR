---
title: Δεν είναι δυνατός ο καθορισμός ή η προβολή της πολιτικής AllowSelfServicePurchase
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
- "9001212"
- "3526"
ms.openlocfilehash: 5ec16b3071f95ef52af2771e95137116222a3c5b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47735199"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="7f180-102">Δεν είναι δυνατός ο καθορισμός ή η προβολή της πολιτικής AllowSelfServicePurchase</span><span class="sxs-lookup"><span data-stu-id="7f180-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="7f180-103">Όταν επιχειρείτε να καθορίσετε ή να προβάλετε την πολιτική AllowSelfServicePurchase, λαμβάνετε το ακόλουθο μήνυμα σφάλματος:</span><span class="sxs-lookup"><span data-stu-id="7f180-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="7f180-104">*HandleError: δεν ήταν δυνατή η ανάκτηση της πολιτικής προϊόντος με το PolicyId ' AllowSelfServicePurchase ', μήνυμα-η υποκείμενη σύνδεση έκλεισε: Παρουσιάστηκε μη αναμενόμενο σφάλμα σε μια αποστολή.*</span><span class="sxs-lookup"><span data-stu-id="7f180-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="7f180-105">Αυτό μπορεί να οφείλεται σε μια παλαιότερη έκδοση της ασφάλειας επιπέδου μεταφοράς (TLS).</span><span class="sxs-lookup"><span data-stu-id="7f180-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="7f180-106">Για να συνδέσετε την υπηρεσία MSCommerce, πρέπει να χρησιμοποιήσετε το TLS 1,2 ή νεότερη.</span><span class="sxs-lookup"><span data-stu-id="7f180-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="7f180-107">Δοκιμάστε τα παρακάτω βήματα για να ενεργοποιήσετε/Ορίστε το πρωτόκολλο TLS στο 1,2, επαληθεύστε και προσπαθήστε ξανά.</span><span class="sxs-lookup"><span data-stu-id="7f180-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="7f180-108">Στη γραμμή εντολών PowerShell (PS C: \) Πληκτρολογήστε την ακόλουθη εντολή για να καθορίσετε το πρωτόκολλο TLS στην έκδοση 1,2:</span><span class="sxs-lookup"><span data-stu-id="7f180-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="7f180-109">Επαληθεύστε τα πρωτόκολλα TLS που χρησιμοποιούνται, με την ακόλουθη εντολή:</span><span class="sxs-lookup"><span data-stu-id="7f180-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="7f180-110">Επαναλάβετε τις εντολές λήψη ή ενημέρωση, ανάλογα με τις ανάγκες.</span><span class="sxs-lookup"><span data-stu-id="7f180-110">Retry the Get or Update commands as needed.</span></span>

