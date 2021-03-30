---
title: Ρύθμιση παραμέτρων προστασίας προσωπικών δεδομένων στον Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004632"
- "8367"
ms.openlocfilehash: 2367a7a55d1837fa7c7095fd0ac10ff1cf7ae72d
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405108"
---
# <a name="configure-privacy-settings-in-microsoft-edge"></a><span data-ttu-id="fbf55-102">Ρύθμιση παραμέτρων προστασίας προσωπικών δεδομένων στον Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="fbf55-102">Configure privacy settings in Microsoft Edge</span></span>

<span data-ttu-id="fbf55-103">Από προεπιλογή, εάν ο Microsoft Edge έχει αναπτυχθεί σε πλατφόρμες που δεν είναι windows, τα διαγνωστικά δεδομένα και οι πληροφορίες τοποθεσίας δεν αποστέλλονται στη Microsoft.</span><span class="sxs-lookup"><span data-stu-id="fbf55-103">By default, if Microsoft Edge is deployed on non-Windows platforms, diagnostic data and site information aren't sent to Microsoft.</span></span> <span data-ttu-id="fbf55-104">Ωστόσο, εάν ο Microsoft Edge έχει αναπτυχθεί στα Windows 10, τα διαγνωστικά δεδομένα και οι πληροφορίες τοποθεσίας αποστέλλονται σύμφωνα με τις ρυθμίσεις δεδομένων [διαγνωστικών των Windows των χρηστών.](https://go.microsoft.com/fwlink/?linkid=2132472)</span><span class="sxs-lookup"><span data-stu-id="fbf55-104">However, if Microsoft Edge is deployed on Windows 10, diagnostic data and site information are sent according to users' [Windows Diagnostic data settings](https://go.microsoft.com/fwlink/?linkid=2132472).</span></span>

<span data-ttu-id="fbf55-105">Για να ρυθμίσετε τον τρόπο με τον οποίο ο Microsoft Edge χειρίζεται τη συλλογή δεδομένων για τον οργανισμό σας, χρησιμοποιήστε τις ακόλουθες πολιτικές ομάδας:</span><span class="sxs-lookup"><span data-stu-id="fbf55-105">To configure how Microsoft Edge handles data collection for your organization, use the following group policies:</span></span>
- <span data-ttu-id="fbf55-106">[Η δυνατότητα MetricsReportingEnabled ενεργοποιεί](https://go.microsoft.com/fwlink/?linkid=2132470) την αναφορά της χρήσης και των δεδομένων που σχετίζονται με σφάλμα.</span><span class="sxs-lookup"><span data-stu-id="fbf55-106">[MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) turns on reporting of usage and crash-related data.</span></span>
- <span data-ttu-id="fbf55-107">[Η sendSiteInfoToImproveServices στέλνει πληροφορίες τοποθεσίας](https://go.microsoft.com/fwlink/?linkid=2132470) που χρησιμοποιούνται για τη βελτίωση των υπηρεσιών της Microsoft.</span><span class="sxs-lookup"><span data-stu-id="fbf55-107">[SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) sends site information used to improve Microsoft services.</span></span>

<span data-ttu-id="fbf55-108">Για να μάθετε περισσότερα, ανατρέξτε στο θέμα [Ρύθμιση παραμέτρων πολιτικής.](https://go.microsoft.com/fwlink/?linkid=2132577)</span><span class="sxs-lookup"><span data-stu-id="fbf55-108">To learn more, see [Configure policy settings](https://go.microsoft.com/fwlink/?linkid=2132577).</span></span>
