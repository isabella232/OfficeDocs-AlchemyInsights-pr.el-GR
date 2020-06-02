---
title: Ζητήματα σύνδεσης σχεδίασης του SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 01ccc6bc28148f397fb6cd2b7a0eaaeb5b51973f
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511544"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="d955c-102">Ζητήματα σύνδεσης σχεδίασης του SharePoint</span><span class="sxs-lookup"><span data-stu-id="d955c-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="d955c-103">Εάν το SharePoint Designer αντιμετωπίζει προβλήματα σύνδεσης σε τοποθεσίες του SharePoint, δοκιμάστε τις ακόλουθες κοινές λύσεις.</span><span class="sxs-lookup"><span data-stu-id="d955c-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="d955c-104">Βήμα 1: Βεβαιωθείτε ότι το SharePoint Designer 2013 ενημερώνεται με το [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) και την ενημερωμένη έκδοση 2 [Αυγούστου 2016 για το SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span><span class="sxs-lookup"><span data-stu-id="d955c-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="d955c-105">Βήμα 2: Απαλοιφή των τοπικών αρχείων προσωρινής αποθήκευσης:</span><span class="sxs-lookup"><span data-stu-id="d955c-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="d955c-106">Κλείστε το SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="d955c-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="d955c-107">Στον τοπικό υπολογιστή, καταργήστε όλα τα αρχεία που βρίσκονται σε κάθε έναν από τους ακόλουθους φακέλους.</span><span class="sxs-lookup"><span data-stu-id="d955c-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="d955c-108">%APPDATA%\Επεκτάσεις διακομιστή Web\Cache</span><span class="sxs-lookup"><span data-stu-id="d955c-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="d955c-109">%APPDATA%\Microsoft\Σχεδιαστής του SharePoint\Cache συγκρότησης διακομιστή μεσολάβησης</span><span class="sxs-lookup"><span data-stu-id="d955c-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="d955c-110">%ΠΡΟΦΊΛ ΧΡΗΣΤΗΣ%\Δεδομένα εφαρμογών\Τοπικές\Microsoft\Cache τοποθεσιών Web</span><span class="sxs-lookup"><span data-stu-id="d955c-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="d955c-111">Ανοίξτε το SharePoint Designer 2013 και πληκτρολογήστε ξανά το λογαριασμό για να δείτε αν λειτουργεί.</span><span class="sxs-lookup"><span data-stu-id="d955c-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="d955c-112">Βήμα 3: [Ενεργοποίηση σύγχρονου ελέγχου ταυτότητας για το Office 2013 σε συσκευές των Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="d955c-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>

<span data-ttu-id="d955c-113">Βήμα 4: Οι διαχειριστές θα πρέπει να **επιτρέψουν την προσαρμοσμένη δέσμη ενεργειών** στις ρυθμίσεις του Κέντρου διαχείρισης του SharePoint για να επιτρέψουν τη σύνδεση του SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="d955c-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="d955c-114">Ανατρέξτε [στο θέμα Να επιτρέπεται ή να αποτρέπεται η προσαρμοσμένη δέσμη ενεργειών](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) για περισσότερες πληροφορίες.</span><span class="sxs-lookup"><span data-stu-id="d955c-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


