---
title: Ρύθμιση παραμέτρων εξαιρέσεων για σάρωση του Microsoft Defender ATP
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6027"
- "9001464"
ms.openlocfilehash: 912e77b9b1a149fef373f2d0814fb2f0671a48c6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "50713573"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="82e31-102">Ρύθμιση παραμέτρων εξαιρέσεων για σάρωση του Microsoft Defender ATP</span><span class="sxs-lookup"><span data-stu-id="82e31-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="82e31-103">Γενικά, μπορείτε να εξαιρέσετε ορισμένες επεκτάσεις αρχείων και θέσεις φακέλων από τις σαρώσεις ATP του Microsoft Defender.</span><span class="sxs-lookup"><span data-stu-id="82e31-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="82e31-104">Μπορείτε επίσης να ρυθμίσετε τις παραμέτρους εξαιρέσεων για αρχεία που ανοίγονται με συγκεκριμένες διαδικασίες.</span><span class="sxs-lookup"><span data-stu-id="82e31-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="82e31-105">Για περισσότερες πληροφορίες, ανατρέξτε στην ενότητα ["Ρύθμιση](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) παραμέτρων και επικύρωση εξαιρέσεων με βάση την επέκταση αρχείου και τη θέση φακέλου" και ρυθμίστε τις παραμέτρους εξαιρέσεων για αρχεία [που ανοίγονται με διαδικασίες.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="82e31-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="82e31-106">Για να ρυθμίσετε τις παραμέτρους των εξαιρέσεων για τον **Windows Server 2016 και 2019,** ανατρέξτε στο θέμα Ρύθμιση παραμέτρων των εξαιρέσεων προστασίας του Microsoft Defender από [ιούς στον Windows Server.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="82e31-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="82e31-107">**Mac**</span><span class="sxs-lookup"><span data-stu-id="82e31-107">**Mac**</span></span>

<span data-ttu-id="82e31-108">Για λεπτομέρειες σχετικά με τους υποστηριζόμενους τύπους εξαίρεσης [](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) και τη ρύθμιση παραμέτρων μιας λίστας εξαιρέσεων για Mac, ανατρέξτε στους υποστηριζόμενους τύπους εξαίρεσης και στον τρόπο ρύθμισης [παραμέτρων της λίστας εξαιρέσεων.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions)</span><span class="sxs-lookup"><span data-stu-id="82e31-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="82e31-109">**Σημείωση** Μπορείτε επίσης να επικυρώσετε λίστες εξαιρέσεων χρησιμοποιώντας το αρχείο δοκιμής EICAR.</span><span class="sxs-lookup"><span data-stu-id="82e31-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="82e31-110">Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα Επικύρωση λιστών εξαιρέσεων με το αρχείο δοκιμής EICAR.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file)</span><span class="sxs-lookup"><span data-stu-id="82e31-110">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="82e31-111">**Linux**</span><span class="sxs-lookup"><span data-stu-id="82e31-111">**Linux**</span></span>

<span data-ttu-id="82e31-112">Για λεπτομέρειες σχετικά με τους υποστηριζόμενους τύπους εξαίρεσης [](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) και τη ρύθμιση παραμέτρων μιας λίστας εξαιρέσεων για Linux, ανατρέξτε στο θέμα "Υποστηριζόμενοι τύποι εξαίρεσης" και "Ρύθμιση παραμέτρων και επικύρωση εξαιρέσεων για [το Microsoft Defender ATP για Linux".](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions)</span><span class="sxs-lookup"><span data-stu-id="82e31-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="82e31-113">**Σημείωση** Μπορείτε επίσης να επικυρώσετε λίστες εξαιρέσεων χρησιμοποιώντας το αρχείο δοκιμής EICAR.</span><span class="sxs-lookup"><span data-stu-id="82e31-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="82e31-114">Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα Επικύρωση λιστών εξαιρέσεων με το αρχείο δοκιμής EICAR.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file)</span><span class="sxs-lookup"><span data-stu-id="82e31-114">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 