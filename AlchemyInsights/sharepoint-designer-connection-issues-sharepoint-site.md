---
title: Προβλήματα σύνδεσης του SharePoint Designer
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 997ba3de58485d4fe6d24b926c33348378af8cd3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727171"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="a8378-102">Προβλήματα σύνδεσης του SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="a8378-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="a8378-103">Εάν το SharePoint Designer αντιμετωπίζει προβλήματα σύνδεσης σε τοποθεσίες του SharePoint, δοκιμάστε τις παρακάτω συνηθισμένες λύσεις.</span><span class="sxs-lookup"><span data-stu-id="a8378-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="a8378-104">Βήμα 1: Επαληθεύστε ότι το SharePoint Designer 2013 ενημερώνεται με το [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) και την [ενημέρωση 2 Αυγούστου 2016 για το sharepoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span><span class="sxs-lookup"><span data-stu-id="a8378-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="a8378-105">Βήμα 2: Καταργήστε την εκκαθάριση των αρχείων της τοπικής μνήμης cache:</span><span class="sxs-lookup"><span data-stu-id="a8378-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="a8378-106">Κλείστε το SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="a8378-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="a8378-107">Στον τοπικό υπολογιστή, καταργήστε όλα τα αρχεία που βρίσκονται σε κάθε έναν από τους παρακάτω φακέλους.</span><span class="sxs-lookup"><span data-stu-id="a8378-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="a8378-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span><span class="sxs-lookup"><span data-stu-id="a8378-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="a8378-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span><span class="sxs-lookup"><span data-stu-id="a8378-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="a8378-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="a8378-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="a8378-111">Ανοίξτε το SharePoint Designer 2013 και εισαγάγετε ξανά τον λογαριασμό για να δείτε εάν λειτουργεί.</span><span class="sxs-lookup"><span data-stu-id="a8378-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="a8378-112">Βήμα 3: [Ενεργοποίηση του σύγχρονου ελέγχου ταυτότητας για το Office 2013 σε συσκευές Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="a8378-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>

<span data-ttu-id="a8378-113">Βήμα 4: οι διαχειριστές θα πρέπει να **επιτρέψουν την προσαρμοσμένη δέσμη ενεργειών** στις ρυθμίσεις του κέντρου διαχείρισης του SharePoint, ώστε να επιτρέπεται η σύνδεση του SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="a8378-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="a8378-114">Ανατρέξτε στο θέμα να [επιτρέπεται ή να εμποδίζεται η προσαρμοσμένη δέσμη ενεργειών](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) για περισσότερες πληροφορίες.</span><span class="sxs-lookup"><span data-stu-id="a8378-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


