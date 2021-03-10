---
title: Ρύθμιση παραμέτρων και επικύρωση εξαιρέσεων για MDATP σε υπολογιστή Linux
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
ms.openlocfilehash: 4fad0a513f7c6d2f0337019488a4055c25e1650d
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50694263"
---
# <a name="configure-and-validate-exclusions-for-mdatp-on-a-linux-machine"></a><span data-ttu-id="cd759-102">Ρύθμιση παραμέτρων και επικύρωση εξαιρέσεων για MDATP σε υπολογιστή Linux</span><span class="sxs-lookup"><span data-stu-id="cd759-102">Configure and validate exclusions for MDATP on a Linux machine</span></span>

<span data-ttu-id="cd759-103">Μπορείτε να εξαιρέσετε ορισμένα αρχεία, φακέλους, διεργασίες και αρχεία που έχουν ανοιχτεί με διαδικασίες από τις σαρώσεις MDATP.</span><span class="sxs-lookup"><span data-stu-id="cd759-103">You can exclude certain files, folders, processes, and process-opened files from MDATP scans.</span></span> <span data-ttu-id="cd759-104">Οι εξαιρέσεις βοηθούν στην αποτροπή εσφαλμένου εντοπισμού λογισμικού και αρχείων μοναδικών ή προσαρμοσμένων για τον οργανισμό σας.</span><span class="sxs-lookup"><span data-stu-id="cd759-104">Exclusions help prevent incorrect detection of software and files unique or customized to your organization.</span></span> <span data-ttu-id="cd759-105">Οι εξαιρέσεις βοηθούν επίσης στην αντιμετώπιση προβλημάτων επιδόσεων που προκαλούνται από την MDATP.</span><span class="sxs-lookup"><span data-stu-id="cd759-105">Exclusions also help mitigate performance problems caused by MDATP.</span></span>

<span data-ttu-id="cd759-106">Για να μάθετε περισσότερα, [ανατρέξτε στο θέμα "Ρύθμιση παραμέτρων και επικύρωση εξαιρέσεων για MDATP για Linux".](https://go.microsoft.com/fwlink/?linkid=2144517)</span><span class="sxs-lookup"><span data-stu-id="cd759-106">To learn more, see [Configure and validate exclusions for MDATP for Linux](https://go.microsoft.com/fwlink/?linkid=2144517).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="cd759-107">Οι εξαιρέσεις που περιγράφονται σε αυτό το άρθρο δεν ισχύουν για άλλες δυνατότητες της MDATP για Linux, συμπεριλαμβανομένου του εντοπισμού τελικού σημείου και της απόκρισης (EDR).</span><span class="sxs-lookup"><span data-stu-id="cd759-107">The exclusions described in this article don't apply to other capabilities of MDATP for Linux, including endpoint detection and response (EDR).</span></span> <span data-ttu-id="cd759-108">Τα αρχεία που εξαιρείτε χρησιμοποιώντας τις μεθόδους που περιγράφονται σε αυτό το άρθρο εξακολουθούν να μπορούν να ενεργοποιήσουν ειδοποιήσεις EDR και άλλες δυνατότητες εντοπισμού.</span><span class="sxs-lookup"><span data-stu-id="cd759-108">Files that you exclude by using the methods described in this article can still trigger EDR alerts and other detection capabilities.</span></span>
