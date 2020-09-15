---
title: Ενεργοποίηση του Office 365 ATP για το SharePoint, το OneDrive και το Microsoft teams
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
ms.openlocfilehash: c84458622ae86bcf0f9f541a3a209b4f0ff2fc3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709907"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="c86b5-102">Ενεργοποίηση του Office 365 προηγμένη προστασία από απειλές για το SharePoint Online, το OneDrive και το Microsoft teams</span><span class="sxs-lookup"><span data-stu-id="c86b5-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="c86b5-103">Μεταβείτε https://protection.office.com και πραγματοποιήστε είσοδο.</span><span class="sxs-lookup"><span data-stu-id="c86b5-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="c86b5-104">Επιλέξτε **Threat management**  >  **Policy**  >  **ασφαλή συνημμένα**πολιτικής διαχείρισης απειλών.</span><span class="sxs-lookup"><span data-stu-id="c86b5-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="c86b5-105">Επιλέξτε **Ενεργοποίηση ATP για το SharePoint, το OneDrive και το Microsoft teams**και, στη συνέχεια, κάντε κλικ στην επιλογή **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="c86b5-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="c86b5-106">Συνιστάται Ως καθολικός διαχειριστής ή διαχειριστής του SharePoint Online, εκτελέστε το cmdlet [συνόλου-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) με την παράμετρο **DisallowInfectedFileDownload** ρυθμισμένη στην *τιμή TRUE*.</span><span class="sxs-lookup"><span data-stu-id="c86b5-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="c86b5-107">Συνιστάται [Ρύθμιση ειδοποιήσεων](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) για αρχεία που έχουν εντοπιστεί.</span><span class="sxs-lookup"><span data-stu-id="c86b5-107">(Recommended) [Set up alerts](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="c86b5-108">Το ATP δεν θα σαρώσει όλα τα αρχεία στο SharePoint Online, το OneDrive ή το Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="c86b5-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="c86b5-109">Τα αρχεία σαρώνονται ασύγχρονα, μέσω μιας διαδικασίας που χρησιμοποιεί συμβάντα δραστηριοτήτων κοινής χρήσης και δραστηριοτήτων επισκεπτών, μαζί με έξυπνα ευρετικά στοιχεία και σήματα απειλών για τον εντοπισμό κακόβουλων αρχείων.</span><span class="sxs-lookup"><span data-stu-id="c86b5-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="c86b5-110">Ανατρέξτε στο θέμα [ATP για SharePoint, OneDrive και Microsoft teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="c86b5-110">See [ATP for SharePoint, OneDrive, and Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>