---
title: Ρύθμιση παραμέτρων εξαιρέσεων για Microsoft Defender ATP σάρωσης
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
ms.openlocfilehash: 5eb18f4133aca93c1506f4975c8d0567bede8d57
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543685"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="e4eba-102">Ρύθμιση παραμέτρων εξαιρέσεων για Microsoft Defender ATP σάρωσης</span><span class="sxs-lookup"><span data-stu-id="e4eba-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="e4eba-103">Γενικά, μπορείτε να εξαιρέσετε ορισμένες επεκτάσεις αρχείων και θέσεις φακέλων από Microsoft Defender ATP σαρώσεις.</span><span class="sxs-lookup"><span data-stu-id="e4eba-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="e4eba-104">Μπορείτε επίσης να ρυθμίσετε τις παραμέτρους εξαιρέσεων για αρχεία που ανοίγουν από συγκεκριμένες διαδικασίες.</span><span class="sxs-lookup"><span data-stu-id="e4eba-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="e4eba-105">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα, [Ρύθμιση](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) παραμέτρων και επικύρωση εξαιρέσεων με βάση την επέκταση αρχείου και τη θέση φακέλου και Ρύθμιση παραμέτρων [εξαιρέσεων για αρχεία που ανοίγουν από διαδικασίες.](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="e4eba-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="e4eba-106">Για να ρυθμίσετε τις παραμέτρους **εξαιρέσεων για Windows Server 2016 και 2019,** ανατρέξτε στο θέμα [Ρύθμιση παραμέτρων Προστασία του Microsoft Defender από ιούς εξαιρέσεων στον Windows Server.](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="e4eba-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="e4eba-107">**Mac**</span><span class="sxs-lookup"><span data-stu-id="e4eba-107">**Mac**</span></span>

<span data-ttu-id="e4eba-108">Για λεπτομέρειες σχετικά με τους υποστηριζόμενους τύπους αποκλεισμού και [](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) τη ρύθμιση παραμέτρων μιας λίστας εξαιρέσεων για Mac, ανατρέξτε στο θέμα Υποστηριζόμενοι τύποι αποκλεισμού και Τρόπος ρύθμισης παραμέτρων [της λίστας εξαιρέσεων.](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions)</span><span class="sxs-lookup"><span data-stu-id="e4eba-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="e4eba-109">**Σημείωση** Μπορείτε επίσης να επικυρώσετε λίστες εξαιρέσεων χρησιμοποιώντας το αρχείο ελέγχου EICAR.</span><span class="sxs-lookup"><span data-stu-id="e4eba-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="e4eba-110">Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα Επικύρωση λιστών εξαιρέσεων με το αρχείο δοκιμής EICAR.](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file)</span><span class="sxs-lookup"><span data-stu-id="e4eba-110">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="e4eba-111">**Linux**</span><span class="sxs-lookup"><span data-stu-id="e4eba-111">**Linux**</span></span>

<span data-ttu-id="e4eba-112">Για λεπτομέρειες σχετικά με τους υποστηριζόμενους τύπους αποκλεισμού και [](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) τη ρύθμιση παραμέτρων μιας λίστας εξαιρέσεων για Linux, ανατρέξτε στο θέμα Υποστηριζόμενοι τύποι αποκλεισμού και Ρύθμιση παραμέτρων και επικύρωση εξαιρέσεων [για Microsoft Defender ATP για Linux.](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions)</span><span class="sxs-lookup"><span data-stu-id="e4eba-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="e4eba-113">**Σημείωση** Μπορείτε επίσης να επικυρώσετε λίστες εξαιρέσεων χρησιμοποιώντας το αρχείο ελέγχου EICAR.</span><span class="sxs-lookup"><span data-stu-id="e4eba-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="e4eba-114">Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα Επικύρωση λιστών εξαιρέσεων με το αρχείο δοκιμής EICAR.](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file)</span><span class="sxs-lookup"><span data-stu-id="e4eba-114">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 