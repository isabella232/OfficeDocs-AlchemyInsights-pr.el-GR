---
title: Δεν υπάρχουν αποτελέσματα αναζήτησης περιεχομένου
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 9f2c0273762f1a4a2b905487f461dc1d05db9209
ms.sourcegitcommit: 8f97342d8b46ab05f1e89018473caad9d35431df
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 07/19/2019
ms.locfileid: "35800362"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="fd244-102">Δεν υπάρχουν αποτελέσματα από περιεχομένου αναζήτησης-ΕΞΑΓΩΓΕΣ</span><span class="sxs-lookup"><span data-stu-id="fd244-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="fd244-103">Ζητήματα με περιεχομένου αναζήτησης/εξαγωγές δεν επιστρέφει δεδομένα ίσως οφείλεται σε ορισμένες φίλτρο ασφαλείας συμμόρφωσης που ήταν εγκατάστασης (Setup) από μια συγκεκριμένη Admin και δεν ανακοινώνουν όλα "διαχειριστές".</span><span class="sxs-lookup"><span data-stu-id="fd244-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="fd244-104">Για να επιλύσετε αυτό το πρόβλημα, ελέγξτε για να δείτε εάν υπάρχουν φίλτρα ασφαλείας συμμόρφωσης που μπορεί να προκαλούν αυτό:</span><span class="sxs-lookup"><span data-stu-id="fd244-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="fd244-105">Συνδεθείτε με ασφάλεια και Powershell συμμόρφωση παραγωγής</span><span class="sxs-lookup"><span data-stu-id="fd244-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="fd244-106">Εκτελέστε τις ακόλουθες commandlets:</span><span class="sxs-lookup"><span data-stu-id="fd244-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="fd244-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="fd244-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="fd244-108">Get-ComplianceSecurityFilter-$org την εταιρεία</span><span class="sxs-lookup"><span data-stu-id="fd244-108">Get-ComplianceSecurityFilter -Organization $org</span></span>