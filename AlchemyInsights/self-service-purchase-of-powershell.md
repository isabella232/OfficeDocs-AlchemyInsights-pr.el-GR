---
title: Αγορά από το powerShell από το web
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
- "3516"
ms.openlocfilehash: 48b5b0a1be1bc03d45a531a1093f18a3f750c37d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51797721"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="491c1-102">Αγορά από το powerShell από το web</span><span class="sxs-lookup"><span data-stu-id="491c1-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="491c1-103">Για να χρησιμοποιήσετε τη λειτουργική μονάδα MSCommerce PowerShell, πρέπει να την εγκαταστήσετε σε μια συσκευή Windows 10 με TLS 1.2 (απαιτούνται δικαιώματα τοπικού διαχειριστή).</span><span class="sxs-lookup"><span data-stu-id="491c1-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="491c1-104">Εισαγωγή και σύνδεση με τη λειτουργική μονάδα MSCommerce.</span><span class="sxs-lookup"><span data-stu-id="491c1-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="491c1-105">Όταν σας ζητηθεί να συνδεθείτε, θα πρέπει να χρησιμοποιήσετε διαπιστευτήρια ρόλου καθολικού ή διαχειριστή χρέωσης.</span><span class="sxs-lookup"><span data-stu-id="491c1-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="491c1-106">Εάν δεν έχετε TLS 1.2, ενδέχεται να εμφανιστεί το ακόλουθο σφάλμα κατά την προσπάθεια λήψης ή ενημέρωσης της πολιτικής:</span><span class="sxs-lookup"><span data-stu-id="491c1-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="491c1-107">*ErrorMessage -Η υποκείμενη σύνδεση έκλεισε: Παρουσιάστηκε μη αναμενόμενο σφάλμα κατά την αποστολή.*</span><span class="sxs-lookup"><span data-stu-id="491c1-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>



