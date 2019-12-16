---
title: Ζητήματα σύνδεσης του SharePoint Designer
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
ms.openlocfilehash: 9730bd66afd494385db3de605f5fe68d0f274ed3
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051713"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="730cd-102">Ζητήματα σύνδεσης του SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="730cd-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="730cd-103">Εάν το SharePoint Designer αντιμετωπίζει ζητήματα σύνδεσης σε τοποθεσίες του SharePoint, δοκιμάστε τις ακόλουθες κοινές λύσεις.</span><span class="sxs-lookup"><span data-stu-id="730cd-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="730cd-104">Βήμα 1: Επαληθεύστε ότι το SharePoint Designer 2013 ενημερώνεται με το [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) και το [2 Αυγούστου, 2016 ενημερωμένη έκδοση για το SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span><span class="sxs-lookup"><span data-stu-id="730cd-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="730cd-105">Βήμα 2: απαλοιφή των αρχείων τοπικής μνήμης cache:</span><span class="sxs-lookup"><span data-stu-id="730cd-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="730cd-106">Κλείστε το SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="730cd-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="730cd-107">Στον τοπικό υπολογιστή, καταργήστε όλα τα αρχεία που βρίσκονται σε καθέναν από τους ακόλουθους φακέλους.</span><span class="sxs-lookup"><span data-stu-id="730cd-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="730cd-108">%AppData%\micssoft\ ρυθμίσεις διακομιστή Web \ cache</span><span class="sxs-lookup"><span data-stu-id="730cd-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="730cd-109">%Appdats\micsss\ σχεδίαση</span><span class="sxs-lookup"><span data-stu-id="730cd-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="730cd-110">%Profile\applods\sooms\ μικρολογισμικός</span><span class="sxs-lookup"><span data-stu-id="730cd-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="730cd-111">Ανοίξτε το SharePoint Designer 2013 και εισαγάγετε ξανά το λογαριασμό για να δείτε αν λειτουργεί.</span><span class="sxs-lookup"><span data-stu-id="730cd-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="730cd-112">Βήμα 3: [Ενεργοποίηση σύγχρονου ελέγχου ταυτότητας για το Office 2013 σε συσκευές Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="730cd-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span></span>

<span data-ttu-id="730cd-113">Βήμα 4: οι διαχειριστές θα πρέπει να **επιτρέψετε προσαρμοσμένη δέσμη ενεργειών** στις ρυθμίσεις του κέντρου διαχείρισης του SharePoint για να επιτρέψετε τη σύνδεση του SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="730cd-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="730cd-114">Δείτε να [επιτρέπεται ή να αποτρέπεται η προσαρμοσμένη δέσμη ενεργειών](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) για περισσότερες πληροφορίες.</span><span class="sxs-lookup"><span data-stu-id="730cd-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


