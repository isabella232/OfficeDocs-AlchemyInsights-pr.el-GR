---
title: Συσκευές εκτός των Windows από την Προηγμένη προστασία του Microsoft Defender από απειλές (ATP)
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
ms.openlocfilehash: 435957c555cd80155a985a49bd94b041a4ada31d
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693813"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a><span data-ttu-id="d5b89-102">Συσκευές εκτός των Windows από την Προηγμένη προστασία του Microsoft Defender από απειλές (ATP)</span><span class="sxs-lookup"><span data-stu-id="d5b89-102">Offboard non-Windows devices from Microsoft Defender Advanced Threat Protection (ATP)</span></span>

<span data-ttu-id="d5b89-103">Αυτό μπορεί να γίνει ως εξής:</span><span class="sxs-lookup"><span data-stu-id="d5b89-103">Here's how:</span></span>

1. <span data-ttu-id="d5b89-104">Ακολουθήστε την τεκμηρίωση άλλου κατασκευαστή για την αποσύνδεση της λύσης τρίτου από το Microsoft Defender ATP.</span><span class="sxs-lookup"><span data-stu-id="d5b89-104">Follow the third-party documentation for disconnecting the third-party solution from Microsoft Defender ATP.</span></span>
2. <span data-ttu-id="d5b89-105">Από το μισθωτή της υπηρεσίας καταλόγου Azure Active Directory, καταργήστε τα δικαιώματα για τη λύση τρίτου κατασκευαστή:</span><span class="sxs-lookup"><span data-stu-id="d5b89-105">From your Azure Active Directory tenant, remove permissions for the third-party solution:</span></span>

    1. <span data-ttu-id="d5b89-106">Πραγματοποιήστε είσοδο στην [πύλη Azure.](https://go.microsoft.com/fwlink/?linkid=2125612)</span><span class="sxs-lookup"><span data-stu-id="d5b89-106">Sign in to the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2125612).</span></span>
    1. <span data-ttu-id="d5b89-107">Επιλέξτε όλες **τις υπηρεσίες** Azure  >  **Active Directory** Enterprise  >  **Applications.**</span><span class="sxs-lookup"><span data-stu-id="d5b89-107">Select **All services** > **Azure Active Directory** > **Enterprise Applications**.</span></span>
    1. <span data-ttu-id="d5b89-108">Επιλέξτε την εφαρμογή της οποία θέλετε να απενεργοποιήσετε.</span><span class="sxs-lookup"><span data-stu-id="d5b89-108">Select the application you'd like to offboard.</span></span>
    1. <span data-ttu-id="d5b89-109">Επιλέξτε **"Διαγραφή".**</span><span class="sxs-lookup"><span data-stu-id="d5b89-109">Select **Delete**.</span></span>

<span data-ttu-id="d5b89-110">Για να μάθετε περισσότερα, ανατρέξτε [στο θέμα "Συσκευές εκτός πίνακα εκτός των Windows".](https://go.microsoft.com/fwlink/?linkid=2143630)</span><span class="sxs-lookup"><span data-stu-id="d5b89-110">To learn more, see [Offboard non-Windows devices](https://go.microsoft.com/fwlink/?linkid=2143630).</span></span>
