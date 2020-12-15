---
title: Ρύθμιση παραμέτρων προστασίας προσωπικών δεδομένων για το Microsoft Edge
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003843"
- "6892"
ms.openlocfilehash: dcd1d91dcde1f585caf0e1e3af30946513a0f26c
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677791"
---
# <a name="microsoft-edge-configure-privacy-settings"></a><span data-ttu-id="6b135-102">Ρύθμιση παραμέτρων προστασίας προσωπικών δεδομένων για το Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="6b135-102">Microsoft Edge configure privacy settings</span></span>

<span data-ttu-id="6b135-103">Από προεπιλογή, εάν το Microsoft Edge έχει αναπτυχθεί σε πλατφόρμες που δεν είναι Windows, τα διαγνωστικά δεδομένα και οι πληροφορίες τοποθεσίας δεν αποστέλλονται στη Microsoft.</span><span class="sxs-lookup"><span data-stu-id="6b135-103">By default, if Microsoft Edge is deployed on non-Windows platforms, diagnostic data and site information are not sent to Microsoft.</span></span> <span data-ttu-id="6b135-104">Ωστόσο, εάν το Microsoft Edge αναπτύσσεται στα Windows 10, τα διαγνωστικά δεδομένα και οι πληροφορίες τοποθεσίας αποστέλλονται σύμφωνα με [τις ρυθμίσεις δεδομένων διαγνωστικών των Windows των](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization)χρηστών.</span><span class="sxs-lookup"><span data-stu-id="6b135-104">However, if Microsoft Edge is deployed on Windows 10, diagnostic data and site information are sent according to users' [Windows Diagnostic data settings](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization).</span></span>

<span data-ttu-id="6b135-105">Για να ρυθμίσετε τον τρόπο με τον οποίο το Microsoft Edge χειρίζεται τη συλλογή δεδομένων για τον οργανισμό σας, χρησιμοποιήστε τις ακόλουθες πολιτικές ομάδας:</span><span class="sxs-lookup"><span data-stu-id="6b135-105">To configure how Microsoft Edge handles data collection for your organization, use the following group policies:</span></span>
- <span data-ttu-id="6b135-106">[MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): αυτή η πολιτική ενεργοποιεί την αναφορά των δεδομένων σχετικά με τη χρήση και τη συντριβή.</span><span class="sxs-lookup"><span data-stu-id="6b135-106">[MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): This policy enables reporting of usage and crash-related data.</span></span>
- <span data-ttu-id="6b135-107">[SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): αυτή η πολιτική στέλνει πληροφορίες τοποθεσίας που χρησιμοποιούνται για τη βελτίωση των υπηρεσιών της Microsoft.</span><span class="sxs-lookup"><span data-stu-id="6b135-107">[SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): This policy sends site information that is used to improve Microsoft services.</span></span>

<span data-ttu-id="6b135-108">Για να μάθετε περισσότερα, ανατρέξτε στο θέμα [Ρύθμιση παραμέτρων των ρυθμίσεων πολιτικής](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).</span><span class="sxs-lookup"><span data-stu-id="6b135-108">To learn more, see [Configure policy settings](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).</span></span>