---
title: Σφάλμα επιδιόρθωσης 0x8004de40 στο OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 5da4271f242597b195ef61d553fd4a2ffb313025
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716028"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="86301-102">Σφάλμα επιδιόρθωσης 0x8004de40 στο OneDrive</span><span class="sxs-lookup"><span data-stu-id="86301-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="86301-103">Εάν λάβετε ένα σφάλμα 0x8004de40 με το OneDrive:</span><span class="sxs-lookup"><span data-stu-id="86301-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="86301-104">Επανεκκινήστε τον υπολογιστή που επηρεάζεται ενώ είναι συνδεδεμένος στον τομέα καταλόγου Acitve.</span><span class="sxs-lookup"><span data-stu-id="86301-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="86301-105">Εάν μια επανεκκίνηση δεν διορθώσει το πρόβλημα, αποσυνδέσου και επανασυνδέω τη συσκευή σας από το Azure AD.</span><span class="sxs-lookup"><span data-stu-id="86301-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="86301-106">**Σημείωση**: Θα πρέπει να βρίσκεστε στο εταιρικό σας δίκτυο κατά την εκτέλεση αυτών των βημάτων.</span><span class="sxs-lookup"><span data-stu-id="86301-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="86301-107">Μην εκτελείτε αυτά τα βήματα όταν δεν μπορείτε να συνδεθείτε στην εταιρική υποδομή σας (για παράδειγμα, ενώ ταξιδεύετε).</span><span class="sxs-lookup"><span data-stu-id="86301-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="86301-108">Ανοίξτε μια υπερυψωμένη γραμμή εντολών.</span><span class="sxs-lookup"><span data-stu-id="86301-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="86301-109">Για να ανοίξετε μια γραμμή εντολών με αυξημένα δικαιώματα, κάντε κλικ στην επιλογή - **Έναρξη**, κάντε δεξί κλικ στη **γραμμή εντολών**και, στη συνέχεια, κάντε κλικ στην επιλογή **Εκτέλεση ως διαχειριστής**.</span><span class="sxs-lookup"><span data-stu-id="86301-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="86301-110">Πληκτρολογήστε *dsregcmd /leave* και **πατήστε το πλήκτρο Enter**.</span><span class="sxs-lookup"><span data-stu-id="86301-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="86301-111">Όταν ολοκληρωθεί, πληκτρολογήστε *dsregcmd /join* και **πατήστε το πλήκτρο Enter**.</span><span class="sxs-lookup"><span data-stu-id="86301-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="86301-112">Όταν ολοκληρωθεί, κλείστε τη γραμμή εντολών.</span><span class="sxs-lookup"><span data-stu-id="86301-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="86301-113">Επανεκκινήστε τον υπολογιστή και συνδεθείτε στο OneDrive.</span><span class="sxs-lookup"><span data-stu-id="86301-113">Reboot the computer, and log into OneDrive.</span></span>