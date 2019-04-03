---
title: Ενεργοποίηση Office 365 ATP για SharePoint, OneDrive και ομάδες της Microsoft
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: ae2f574663ae3233a056589c2d5a578171f3b2f4
ms.sourcegitcommit: 601aec31e6556286fe5e0fd62827a037cbb6fe17
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/02/2019
ms.locfileid: "31030974"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="1712d-102">Ενεργοποίηση Office 365 απειλή για προχωρημένους προστασίας για ηλεκτρονική SharePoint, OneDrive και ομάδες της Microsoft</span><span class="sxs-lookup"><span data-stu-id="1712d-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="1712d-103">Μεταβείτε στην https://protection.office.com και να εισέλθετε.</span><span class="sxs-lookup"><span data-stu-id="1712d-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="1712d-104">Επιλέξτε **Διαχείριση απειλή** > **πολιτική** > **Ασφαλή συνημμένα**.</span><span class="sxs-lookup"><span data-stu-id="1712d-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="1712d-105">Επιλέξτε **Ενεργοποίηση αυτόματης ασφάλειας Αμαξοστοιχίας για SharePoint, OneDrive, και ομάδες της Microsoft**και, στη συνέχεια, κάντε κλικ στο κουμπί **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="1712d-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="1712d-106">(Συνιστάται) Ως ένας καθολικός διαχειριστής ή ένας διαχειριστής SharePoint Online, εκτελέστε το cmdlet [Σύνολο SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) με την παράμετρο **DisallowInfectedFileDownload** που έχει οριστεί στην *τιμή true*.</span><span class="sxs-lookup"><span data-stu-id="1712d-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="1712d-107">(Συνιστάται) [Ρύθμιση ειδοποιήσεων](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) για τα αρχεία που εντοπίστηκαν.</span><span class="sxs-lookup"><span data-stu-id="1712d-107">(Recommended) [Set up alerts](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="1712d-108">ATP θα nto σάρωση κάθε αρχείο σε ηλεκτρονική SharePoint, OneDrive ή ομάδες της Microsoft.</span><span class="sxs-lookup"><span data-stu-id="1712d-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="1712d-109">Σάρωση των αρχείων γίνεται ασύγχρονα, μέσω μιας διαδικασίας που χρησιμοποιεί συμβάντα δραστηριότητα κοινής χρήσης και guest, καθώς και έξυπνες λύσεις και σήματα απειλή για τον προσδιορισμό κακόβουλα αρχεία.</span><span class="sxs-lookup"><span data-stu-id="1712d-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="1712d-110">Ανατρέξτε στην ενότητα [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="1712d-110">See [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>