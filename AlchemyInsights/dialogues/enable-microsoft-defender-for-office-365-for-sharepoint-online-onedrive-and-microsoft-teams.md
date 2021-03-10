---
title: Ενεργοποίηση του Microsoft Defender για το Office 365 για το SharePoint Online, το OneDrive και το Microsoft Teams
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 1c29afdcc52e7032fea22d698371677918665fa9
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694041"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="32121-102">Ενεργοποίηση του Microsoft Defender για το Office 365 για το SharePoint Online, το OneDrive και το Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="32121-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive and Microsoft Teams</span></span>

1. <span data-ttu-id="32121-103">Χρησιμοποιώντας τα διαπιστευτήρια καθολικού διαχειριστή ή διαχειριστή ασφάλειας, συνδεθείτε στο Κέντρο ασφάλειας και συμμόρφωσης του [Office 365.](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="32121-103">Using your global admin or security admin credentials, log in to the [Office 365 Security and Compliance Center](https://protection.office.com/).</span></span>
2. <span data-ttu-id="32121-104">Επιλέξτε **"Διαχείριση απειλών"** στο αριστερό τμήμα παραθύρου και, στη συνέχεια, επιλέξτε **"Ασφαλή**  >  [συνημμένα πολιτικής".](https://protection.office.com/safeattachment)</span><span class="sxs-lookup"><span data-stu-id="32121-104">Select **Threat management** in the left pane, and then select **Policy** > [Safe attachments](https://protection.office.com/safeattachment).</span></span>
3. <span data-ttu-id="32121-105">Επιλέξτε **"Ενεργοποίηση του Microsoft Defender για το Office 365 για το SharePoint, το OneDrive** και το Microsoft Teams" και, στη συνέχεια, επιλέξτε **"Αποθήκευση".**</span><span class="sxs-lookup"><span data-stu-id="32121-105">Select **Turn on Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**, and then select **Save**.</span></span>
    > [!TIP]
    >
    > - <span data-ttu-id="32121-106">Ως καθολικός διαχειριστής ή διαχειριστής του SharePoint Online, εκτελέστε το ακόλουθο cmdlet του PowerShell με την παράμετρο **DisallowInfectedFileDownload** να έχει οριστεί στην τιμή *true:* [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)</span><span class="sxs-lookup"><span data-stu-id="32121-106">As a global admin or a SharePoint Online admin, run the following PowerShell cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*: [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)</span></span>
    > - [<span data-ttu-id="32121-107">Ρύθμιση ειδοποιήσεων για τα αρχεία που εντοπίστηκαν</span><span class="sxs-lookup"><span data-stu-id="32121-107">Set up alerts for detected files</span></span>](https://go.microsoft.com/fwlink/?linkid=2092110)

<span data-ttu-id="32121-108">Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα Microsoft Defender για το Office 365 για το SharePoint, το OneDrive και το Microsoft Teams.](https://go.microsoft.com/fwlink/?linkid=2092041)</span><span class="sxs-lookup"><span data-stu-id="32121-108">For more information, see [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041).</span></span>
