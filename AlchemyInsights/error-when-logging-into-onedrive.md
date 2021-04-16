---
title: 0x8004de40 κατά την εκκίνηση του OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813652"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="53cc4-102">0x8004de40 κατά την εκκίνηση του OneDrive</span><span class="sxs-lookup"><span data-stu-id="53cc4-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="53cc4-103">Εάν εμφανιστεί ένα σφάλμα κατά **0x8004de40 σύνδεση** στο OneDrive, επανεκκινήστε τον υπολογιστή ενώ είστε συνδεδεμένοι στον τομέα της εργασίας ή του σχολείου σας.</span><span class="sxs-lookup"><span data-stu-id="53cc4-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="53cc4-104">Εάν εμφανιστεί αυτό το σφάλμα μετά την επανεκκίνηση, δοκιμάστε το ενώ είστε συνδεδεμένοι στον τομέα της εργασίας ή του σχολείου σας:</span><span class="sxs-lookup"><span data-stu-id="53cc4-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="53cc4-105">Κάντε κλικ στην επιλογή "Έναρξη" και πληκτρολογήστε **cmd** ή **γραμμή** εντολών στο πλαίσιο αναζήτησης, κάντε δεξί κλικ στην εφαρμογή γραμμής εντολών και επιλέξτε **"Εκτέλεση ως διαχειριστής".**</span><span class="sxs-lookup"><span data-stu-id="53cc4-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator**.</span></span> <span data-ttu-id="53cc4-106">Εάν σας ζητηθεί κωδικός πρόσβασης διαχειριστή ή επιβεβαίωση, πληκτρολογήστε τον κωδικό πρόσβασης ή κάντε κλικ στην επιλογή **"Να επιτρέπεται".**</span><span class="sxs-lookup"><span data-stu-id="53cc4-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow**.</span></span>  

2. <span data-ttu-id="53cc4-107">Στο παράθυρο της γραμμής εντολών, πληκτρολογήστε **dsregcmd /leave**  και περιμένετε να ολοκληρωθεί η εντολή.</span><span class="sxs-lookup"><span data-stu-id="53cc4-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="53cc4-108">Στη **συνέχεια, πληκτρολογήστε dsregcmd /join** και περιμένετε να ολοκληρωθεί η εντολή.</span><span class="sxs-lookup"><span data-stu-id="53cc4-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="53cc4-109">Επανεκκινήστε τον υπολογιστή σας.</span><span class="sxs-lookup"><span data-stu-id="53cc4-109">Reboot your computer.</span></span>
