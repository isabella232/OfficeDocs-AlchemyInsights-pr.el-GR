---
title: σφάλμα 0x8004de40 κατά την εκκίνηση του OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823048"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="baa09-102">σφάλμα 0x8004de40 κατά την εκκίνηση του OneDrive</span><span class="sxs-lookup"><span data-stu-id="baa09-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="baa09-103">Εάν λάβετε ένα μήνυμα σφάλματος **0x8004de40** κατά τη σύνδεση στο OneDrive, επανεκκινήστε τον υπολογιστή ενώ είστε συνδεδεμένοι στον τομέα της εργασίας ή του σχολείου σας.</span><span class="sxs-lookup"><span data-stu-id="baa09-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="baa09-104">Εάν λάβετε αυτό το σφάλμα μετά την επανεκκίνηση, δοκιμάστε αυτό ενώ είστε συνδεδεμένοι με τον τομέα της εργασίας ή του σχολείου σας:</span><span class="sxs-lookup"><span data-stu-id="baa09-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="baa09-105">Κάντε κλικ στην επιλογή Έναρξη και πληκτρολογήστε **cmd** ή **γραμμή**  εντολών στο πλαίσιο αναζήτησης, κάντε δεξί κλικ στην εφαρμογή γραμμή εντολών και επιλέξτε  **Εκτέλεση ως διαχειριστής** .</span><span class="sxs-lookup"><span data-stu-id="baa09-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator** .</span></span> <span data-ttu-id="baa09-106">Εάν σας ζητηθεί κωδικός πρόσβασης διαχειριστή ή επιβεβαίωση, πληκτρολογήστε τον κωδικό πρόσβασης ή κάντε κλικ στο κουμπί **Αποδοχή** .</span><span class="sxs-lookup"><span data-stu-id="baa09-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow** .</span></span>  

2. <span data-ttu-id="baa09-107">Στο παράθυρο της γραμμής εντολών, πληκτρολογήστε **dsregcmd/Leave**  και περιμένετε να ολοκληρωθεί η εντολή.</span><span class="sxs-lookup"><span data-stu-id="baa09-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="baa09-108">Στη συνέχεια, πληκτρολογήστε **dsregcmd/Join** και περιμένετε να ολοκληρωθεί η εντολή.</span><span class="sxs-lookup"><span data-stu-id="baa09-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="baa09-109">Επανεκκινήστε τον υπολογιστή σας.</span><span class="sxs-lookup"><span data-stu-id="baa09-109">Reboot your computer.</span></span>
