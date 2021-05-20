---
title: Ενεργοποίηση Office 365 ATP για SharePoint, OneDrive και Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: dd367176f8d6f38f1f94ae6627229234f15c81ff
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543928"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="aa5cb-102">Ενεργοποίηση του Microsoft Defender για Office 365 για SharePoint Online, OneDrive και Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="aa5cb-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="aa5cb-103">Μεταβείτε https://protection.office.com και πραγματοποιήστε είσοδο.</span><span class="sxs-lookup"><span data-stu-id="aa5cb-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="aa5cb-104">Επιλέξτε **"Ασφαλή**  >  **συνημμένα πολιτικής** διαχείρισης  >  **απειλών".**</span><span class="sxs-lookup"><span data-stu-id="aa5cb-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="aa5cb-105">Επιλέξτε **"Ενεργοποίηση του Defender" για Office 365 για SharePoint, OneDrive και Microsoft Teams και, στη** συνέχεια, κάντε κλικ στην επιλογή **"Αποθήκευση".**</span><span class="sxs-lookup"><span data-stu-id="aa5cb-105">Select **Turn on Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="aa5cb-106">(Συνιστάται) Ως καθολικός διαχειριστής ή διαχειριστής του SharePoint Online, εκτελέστε το [cmdlet Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) με την παράμετρο **DisallowInfectedFileDownload** να έχει οριστεί σε *true.*</span><span class="sxs-lookup"><span data-stu-id="aa5cb-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="aa5cb-107">(Συνιστάται) [Ρύθμιση ειδοποιήσεων για](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) αρχεία που εντοπίστηκαν.</span><span class="sxs-lookup"><span data-stu-id="aa5cb-107">(Recommended) [Set up alerts](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="aa5cb-108">Ο Microsoft Defender Office 365 δεν θα σαρώνει κάθε αρχείο SharePoint online, OneDrive ή Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="aa5cb-108">Microsoft Defender for Office 365 will not scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="aa5cb-109">Τα αρχεία σαρώνονται ασύγχρονα, μέσω μιας διαδικασίας που χρησιμοποιεί συμβάντα κοινής χρήσης και δραστηριότητας επισκεπτών, καθώς και έξυπνα heuristics και σήματα απειλών για τον προσδιορισμό κακόβουλων αρχείων.</span><span class="sxs-lookup"><span data-stu-id="aa5cb-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="aa5cb-110">Ανατρέξτε [στο θέμα Microsoft Defender για Office 365 για SharePoint, OneDrive και Microsoft Teams.](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)</span><span class="sxs-lookup"><span data-stu-id="aa5cb-110">See [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>