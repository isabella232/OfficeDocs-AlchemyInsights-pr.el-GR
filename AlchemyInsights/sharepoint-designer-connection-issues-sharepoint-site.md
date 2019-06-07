---
title: Τα επίπεδα δικαιωμάτων του SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 356fef8e02f2c1fd9d209c68194685bb0acaa367
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760693"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="c470b-102">Προβλήματα σύνδεσης του SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="c470b-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="c470b-103">Εάν το SharePoint Designer αντιμετωπίζει ζητήματα σύνδεσης σε τοποθεσίες του SharePoint, προσπαθήστε τις ακόλουθες κοινές λύσεις.</span><span class="sxs-lookup"><span data-stu-id="c470b-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please attempt the following common solutions.</span></span>

<span data-ttu-id="c470b-104">Βήμα 1: Βεβαιωθείτε ενημερώνεται το SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="c470b-104">Step 1: Verify SharePoint Designer is updated.</span></span>

- [<span data-ttu-id="c470b-105">Του SharePoint Designer 2013</span><span class="sxs-lookup"><span data-stu-id="c470b-105">SharePoint Designer 2013</span></span>](https://www.microsoft.com/download/details.aspx?id=35491)

- [<span data-ttu-id="c470b-106">Το SharePoint Designer Service Pack 1 (SP1)</span><span class="sxs-lookup"><span data-stu-id="c470b-106">SharePoint Designer Service Pack 1 (SP1)</span></span>](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)

- [<span data-ttu-id="c470b-107">Ενημερωμένη έκδοση για το SharePoint Designer 2013 (KB3114721)</span><span class="sxs-lookup"><span data-stu-id="c470b-107">Update for SharePoint Designer 2013 (KB3114721)</span></span>](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)

<span data-ttu-id="c470b-108">Βήμα 2: Καταργήστε το τοπικό χώρο προσωρινής αποθήκευσης αρχείων</span><span class="sxs-lookup"><span data-stu-id="c470b-108">Step 2: Clear the local cache files</span></span>

- <span data-ttu-id="c470b-109">Κλείσιμο του SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="c470b-109">Close SharePoint Designer 2013.</span></span>

- <span data-ttu-id="c470b-110">Στον τοπικό υπολογιστή, μεταβείτε στους ακόλουθους φακέλους για να καταργήσετε προσωρινά αποθηκευμένα αρχεία.</span><span class="sxs-lookup"><span data-stu-id="c470b-110">On the local computer, browse to the following folders to remove cached files.</span></span>

- <span data-ttu-id="c470b-111">Κάντε κλικ στο κουμπί Έναρξη, εκτέλεση "και" Διαγραφή όλων των αρχείων που βρέθηκαν σε κάθε μία από τις παρακάτω θέσεις.</span><span class="sxs-lookup"><span data-stu-id="c470b-111">Click Start, Run and delete all files found under each of the below locations.</span></span>

<span data-ttu-id="c470b-112">Διακομιστής %APPDATA%\Microsoft\Web Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="c470b-112">%APPDATA%\Microsoft\Web Server Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

<span data-ttu-id="c470b-113">Άνοιγμα του SharePoint Designer 2013 και εισαγάγετε το λογαριασμό ξανά, για να δείτε αν λειτουργεί.</span><span class="sxs-lookup"><span data-stu-id="c470b-113">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="c470b-114">Βήμα 3: [Ενεργοποίηση σύγχρονη ελέγχου ταυτότητας για το Office 2013 σε συσκευές των Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="c470b-114">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)</span></span>

<span data-ttu-id="c470b-115">Βήμα 4: Οι διαχειριστές θα πρέπει να επιτρέψει προσαρμοσμένης δέσμης ενεργειών επιτρέπουν τη σύνδεση του SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="c470b-115">Step 4: Administrators will need to Allow Custom Script to allow the SharePoint Designer connection.</span></span>

<span data-ttu-id="c470b-116">Για λεπτομερή βήματα, παραδείγματα και ζητήματα, δείτε [επιτρέπεται ή να απαγορεύεται η προσαρμοσμένη δέσμη ενεργειών](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="c470b-116">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


