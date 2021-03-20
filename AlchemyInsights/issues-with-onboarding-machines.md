---
title: Προβλήματα με την προσθήκη υπολογιστών στο Microsoft Defender για τελικά σημεία
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 7ccec69f8ab43f277978176519a7f8f8df443846
ms.sourcegitcommit: 1d73771d147325cfd8578e6816becd8331913890
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 03/19/2021
ms.locfileid: "50901567"
---
# <a name="issues-with-onboarding-machines-to-microsoft-defender-for-endpoints"></a><span data-ttu-id="a5c78-102">Προβλήματα με την προσθήκη υπολογιστών στο Microsoft Defender για τελικά σημεία</span><span class="sxs-lookup"><span data-stu-id="a5c78-102">Issues with onboarding machines to Microsoft Defender for Endpoints</span></span>

<span data-ttu-id="a5c78-103">Μπορεί να αντιμετωπίσετε προβλήματα με την προσθήκη υπολογιστών στην υπηρεσία MDE.</span><span class="sxs-lookup"><span data-stu-id="a5c78-103">You might have issues with onboarding machines to MDE service.</span></span> <span data-ttu-id="a5c78-104">Εάν μπορείτε να έχετε πρόσβαση στον υπολογιστή τελικού χρήστη, ακολουθήστε τα παρακάτω βήματα:</span><span class="sxs-lookup"><span data-stu-id="a5c78-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="a5c78-105">Κατεβάστε την τελευταία έκδοση προεπισκόπησης του διαγνωστικού εργαλείου [MDE Client Analyzer](https://aka.ms/betamdeanalyzer).</span><span class="sxs-lookup"><span data-stu-id="a5c78-105">Download the latest preview version of the [MDE Client Analyzer](https://aka.ms/betamdeanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="a5c78-106">Κάντε δεξί κλικ στο **MDEClientAnalyzer.cmd** και επιλέξτε "Εκτέλεση ως διαχειριστής".</span><span class="sxs-lookup"><span data-stu-id="a5c78-106">Right click **MDEClientAnalyzer.cmd** and select ‘Run as administrator’.</span></span>
3. <span data-ttu-id="a5c78-107">Ακολουθήστε τις οδηγίες που προτείνονται στο **MDEClientAnalyzer.htm**.</span><span class="sxs-lookup"><span data-stu-id="a5c78-107">Follow any guidance suggested in **MDEClientAnalyzer.htm**.</span></span>
4. <span data-ttu-id="a5c78-108">Για πιο λεπτομερή αρχεία καταγραφής, ελέγξτε τον υποφάκελο που δημιουργήθηκε με ονομασία **MDEClientAnalyzerResult**.</span><span class="sxs-lookup"><span data-stu-id="a5c78-108">For more verbose logs, review the created sub-folder named **MDEClientAnalyzerResult**.</span></span>
5. <span data-ttu-id="a5c78-109">Εάν χρειάζεστε πρόσθετες οδηγίες, επικοινωνήστε με την [υποστήριξη του Microsoft Defender για τελικό σημείο](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) και δώστε το αρχείο MDEClientAnalyzerResult.zip που προκύπτει για ανάλυση.</span><span class="sxs-lookup"><span data-stu-id="a5c78-109">If additional guidance is needed, contact [Microsoft Defender for Endpoint support](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) and provide the resulting MDEClientAnalyzerResult.zip file for analysis.</span></span>
