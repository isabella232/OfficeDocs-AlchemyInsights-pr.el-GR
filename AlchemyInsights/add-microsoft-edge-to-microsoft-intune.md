---
title: Προσθήκη του Microsoft Edge στο Microsoft Intune
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8240"
- "9004604"
ms.openlocfilehash: d56c65910d1c2170d3e0ce9676e913663701db96
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 02/10/2021
ms.locfileid: "50194508"
---
# <a name="add-microsoft-edge-to-microsoft-intune"></a><span data-ttu-id="3f7c2-102">Προσθήκη του Microsoft Edge στο Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="3f7c2-102">Add Microsoft Edge to Microsoft Intune</span></span>

<span data-ttu-id="3f7c2-103">Για να μπορείτε να αναπτύξετε, να ρυθμίσετε τις παραμέτρους, να παρακολουθήσετε και να προστατεύσετε τον Microsoft Edge για Windows 10, πρέπει πρώτα να τον προσθέσετε στο Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="3f7c2-103">To be able to deploy, configure, monitor, and protect Microsoft Edge for Windows 10, you must first add it to Microsoft Intune.</span></span>

> [!IMPORTANT]
- <span data-ttu-id="3f7c2-104">Το Intune υποστηρίζει τον Microsoft Edge 77 και νεότερες εκδόσεις.</span><span class="sxs-lookup"><span data-stu-id="3f7c2-104">Intune supports Microsoft Edge 77 and later versions.</span></span>
- <span data-ttu-id="3f7c2-105">Το Intune θα εντοπίσει τυχόν προϋπάρχουσα εγκατάσταση του Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="3f7c2-105">Intune will detect any pre-existing installations of Microsoft Edge.</span></span>
- <span data-ttu-id="3f7c2-106">Εάν ο Microsoft Edge είναι εγκατεστημένος στο περιβάλλον χρήστη, μια εγκατάσταση συστήματος θα αντικαταστήσει την εγκατάσταση στο περιβάλλον χρήστη.</span><span class="sxs-lookup"><span data-stu-id="3f7c2-106">If Microsoft Edge is installed in user context, a system installation will overwrite the installation in user context.</span></span>
- <span data-ttu-id="3f7c2-107">Εάν ο Microsoft Edge εγκατασταθεί σε περιβάλλον συστήματος, θα αναφερθεί η επιτυχία της εγκατάστασης.</span><span class="sxs-lookup"><span data-stu-id="3f7c2-107">If Microsoft Edge is installed in system context, the installation success will be reported.</span></span>
- <span data-ttu-id="3f7c2-108">Ο προεγκατεστημένες εκδόσεις του Microsoft Edge 77 και νεότερες εκδόσεις, για όλα τα κανάλια στο περιβάλλον χρήστη, θα αντικατασταθούν με τον Microsoft Edge εγκατεστημένο στο περιβάλλον του συστήματος.</span><span class="sxs-lookup"><span data-stu-id="3f7c2-108">Pre-installed Microsoft Edge 77 and later versions, for all channels in user context, will be overwritten with Microsoft Edge installed in system context.</span></span>

<span data-ttu-id="3f7c2-109">**Προαπαιτούμενο**</span><span class="sxs-lookup"><span data-stu-id="3f7c2-109">**Prerequisite**</span></span>

<span data-ttu-id="3f7c2-110">Windows 10 έκδοση 1709 ή νεότερες εκδόσεις</span><span class="sxs-lookup"><span data-stu-id="3f7c2-110">Windows 10 version 1709 or later versions</span></span>

<span data-ttu-id="3f7c2-111">**Βήματα για προσθήκη του Edge στο Intune**</span><span class="sxs-lookup"><span data-stu-id="3f7c2-111">**Steps to add Edge to Intune**</span></span>

1. <span data-ttu-id="3f7c2-112">[Ρυθμίστε τις παραμέτρους της εφαρμογής στο Intune.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="3f7c2-112">[Configure the app in Intune](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
2. <span data-ttu-id="3f7c2-113">[Ρυθμίστε τις παραμέτρους των πληροφοριών της εφαρμογής.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="3f7c2-113">[Configure the app information](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
3. <span data-ttu-id="3f7c2-114">[Διαμορφώστε τις ρυθμίσεις της εφαρμογής.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="3f7c2-114">[Configure the app settings](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
4. <span data-ttu-id="3f7c2-115">[Επιλέξτε τις ετικέτες εύρους (προαιρετικό).](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="3f7c2-115">[Select the scope tags (optional)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
5. <span data-ttu-id="3f7c2-116">[Προσθέστε την εφαρμογή.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="3f7c2-116">[Add the app](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>

<span data-ttu-id="3f7c2-117">Για περισσότερη βοήθεια, ανατρέξτε στην [αντιμετώπιση προβλημάτων.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="3f7c2-117">For more help, see [Troubleshooting](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>




