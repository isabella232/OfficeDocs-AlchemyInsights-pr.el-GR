---
title: Ενεργοποίηση atp του Office 365 για ομάδες Του SharePoint, OneDrive και Microsoft
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 564a7f1f6a37e64dbd7d679878ebadbbe35f3fa0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506918"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="9635a-102">Ενεργοποίηση της Προηγμένης προστασίας από απειλές του Office 365 για ομάδες του SharePoint Online, του OneDrive και της Microsoft</span><span class="sxs-lookup"><span data-stu-id="9635a-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="9635a-103">Πήγαινε https://protection.office.com και συνδεθείτε.</span><span class="sxs-lookup"><span data-stu-id="9635a-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="9635a-104">Επιλέξτε **Ασφαλή**  >  συνημμένα**πολιτικής**  >  **διαχείρισης**απειλών .</span><span class="sxs-lookup"><span data-stu-id="9635a-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="9635a-105">Επιλέξτε **Ενεργοποίηση atp για ομάδες SharePoint, OneDrive και Microsoft**και, στη συνέχεια, κάντε κλικ στην επιλογή **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="9635a-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="9635a-106">(Συνιστάται) Ως καθολικός διαχειριστής ή διαχειριστής του SharePoint Online, εκτελέστε το cmdlet [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) με την παράμετρο **DisallowInfectedFileDownload** που έχει οριστεί σε *true*.</span><span class="sxs-lookup"><span data-stu-id="9635a-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="9635a-107">(Συνιστάται) [Ρύθμιση ειδοποιήσεων](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) για αρχεία που εντοπίστηκαν.</span><span class="sxs-lookup"><span data-stu-id="9635a-107">(Recommended) [Set up alerts](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="9635a-108">Η ATP θα σαρώσει κάθε αρχείο στο SharePoint Online, το OneDrive ή το Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="9635a-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="9635a-109">Τα αρχεία σαρώνονται ασύγχρονα, μέσω μιας διαδικασίας που χρησιμοποιεί συμβάντα κοινής χρήσης και δραστηριότητας επισκεπτών, μαζί με έξυπνα ευρετική και σήματα απειλής για τον εντοπισμό κακόβουλων αρχείων.</span><span class="sxs-lookup"><span data-stu-id="9635a-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="9635a-110">Ανατρέξτε [στο θέμα ATP για ομάδες του SharePoint, του OneDrive και του Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="9635a-110">See [ATP for SharePoint, OneDrive, and Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>