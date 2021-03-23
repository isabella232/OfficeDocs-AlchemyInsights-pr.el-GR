---
title: Απομακρυσμένη επιδιόρθωση προβλημάτων με την εγκατάσταση συσκευών Windows 10 στην Προηγμένη προστασία από απειλές του Microsoft Defender
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
ms.openlocfilehash: 5473d090f6d4680f9a62f34f943ac6cea53b2079
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746447"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a><span data-ttu-id="6263b-102">Απομακρυσμένη επιδιόρθωση προβλημάτων με την εγκατάσταση συσκευών Windows 10 στην Προηγμένη προστασία από απειλές του Microsoft Defender</span><span class="sxs-lookup"><span data-stu-id="6263b-102">Remotely fix problems with onboarding Windows 10 devices to Microsoft Defender Advanced Threat Protection</span></span>

<span data-ttu-id="6263b-103">Εάν μπορείτε να αποκτήσετε πρόσβαση στον απομακρυσμένο υπολογιστή, ακολουθήστε τα παρακάτω βήματα:</span><span class="sxs-lookup"><span data-stu-id="6263b-103">If you can access the remote computer, follow these steps:</span></span>

1. <span data-ttu-id="6263b-104">Κάντε λήψη του [διαγνωστικού εργαλείου "Ανάλυση συνδεσιμότητας προγράμματος-πελάτη".](https://go.microsoft.com/fwlink/?linkid=2143466)</span><span class="sxs-lookup"><span data-stu-id="6263b-104">Download the [Client Connectivity Analyzer](https://go.microsoft.com/fwlink/?linkid=2143466) diagnostic tool.</span></span>
2. <span data-ttu-id="6263b-105">Εξαγάγετε και εκτελέστε το MDATPAnalyzer.cmd.</span><span class="sxs-lookup"><span data-stu-id="6263b-105">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="6263b-106">Εντοπίστε το αρχείο καταγραφής διαγνωστικών στο φάκελο MDATPClientAnalyzerResult, ο οποίος είναι ο ίδιος φάκελος όπου έγινε λήψη του εργαλείου Analyzer.</span><span class="sxs-lookup"><span data-stu-id="6263b-106">Locate the diagnostic log in the MDATPClientAnalyzerResult folder, which is the same folder where the Analyzer tool was downloaded.</span></span>
4. <span data-ttu-id="6263b-107">Για να βρείτε προβλήματα με τις ρυθμίσεις συνδεσιμότητας ή διακομιστή μεσολάβησης Internet, εξετάστε το αρχείο καταγραφής MDATPClientAnalyzer.txt.</span><span class="sxs-lookup"><span data-stu-id="6263b-107">To find issues with connectivity or Internet proxy settings, review the log file MDATPClientAnalyzer.txt.</span></span>

<span data-ttu-id="6263b-108">Για να μάθετε περισσότερα, ανατρέξτε [στο θέμα Προβλήματα με τους υπολογιστές με πίνακες.](https://go.microsoft.com/fwlink/?linkid=2143634)</span><span class="sxs-lookup"><span data-stu-id="6263b-108">To learn more, see [Issues with onboarding machines](https://go.microsoft.com/fwlink/?linkid=2143634).</span></span>