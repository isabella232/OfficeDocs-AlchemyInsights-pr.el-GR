---
title: Διορθώστε το σφάλμα 0x8004de40 στο OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: aa0e0a63ac1e365a7cdce018626740446040a664
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36755848"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="ce1d1-102">Διορθώστε το σφάλμα 0x8004de40 στο OneDrive</span><span class="sxs-lookup"><span data-stu-id="ce1d1-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="ce1d1-103">Εάν λάβετε ένα σφάλμα 0x8004de40 με το OneDrive:</span><span class="sxs-lookup"><span data-stu-id="ce1d1-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="ce1d1-104">Επανεκκινήστε τον υπολογιστή που επηρεάζεται, ενώ είστε συνδεδεμένοι στον τομέα του καταλόγου</span><span class="sxs-lookup"><span data-stu-id="ce1d1-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="ce1d1-105">Εάν μια επανεκκίνηση δεν διορθώνει το ζήτημα, καταργήστε την ένταξη και επανσυνδεθείτε στη συσκευή σας από το Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ce1d1-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="ce1d1-106">**Σημείωση**: θα πρέπει να βρίσκεστε στο εταιρικό σας δίκτυο κατά την εκτέλεση αυτών των βημάτων.</span><span class="sxs-lookup"><span data-stu-id="ce1d1-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="ce1d1-107">Μην εκτελείτε αυτά τα βήματα όταν δεν μπορείτε να συνδεθείτε με την εταιρική σας υποδομή (για παράδειγμα, ενώ ταξιδεύετε).</span><span class="sxs-lookup"><span data-stu-id="ce1d1-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="ce1d1-108">Ανοίξτε μια γραμμή εντολών με αυξημένα δικαιώματα.</span><span class="sxs-lookup"><span data-stu-id="ce1d1-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="ce1d1-109">Για να ανοίξετε μια αναβαθμισμένη γραμμή εντολών, κάντε κλικ στην επιλογή- **Start**, κάντε δεξιό κλικ στη **γραμμή εντολών**και, στη συνέχεια, κάντε κλικ στο κουμπί **Εκτέλεση ως διαχειριστής**.</span><span class="sxs-lookup"><span data-stu-id="ce1d1-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="ce1d1-110">Πληκτρολογήστε *dsregcmd/αφήστε* και πιέστε το πλήκτρο **ENTER**.</span><span class="sxs-lookup"><span data-stu-id="ce1d1-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="ce1d1-111">Όταν ολοκληρωθεί, πληκτρολογήστε *dsregcmd/συμμετάσχετε* και πιέστε το πλήκτρο **ENTER**.</span><span class="sxs-lookup"><span data-stu-id="ce1d1-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="ce1d1-112">Όταν ολοκληρωθεί, κλείστε τη γραμμή εντολών.</span><span class="sxs-lookup"><span data-stu-id="ce1d1-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="ce1d1-113">Επανεκκινήστε τον υπολογιστή και συνδεθείτε στο OneDrive.</span><span class="sxs-lookup"><span data-stu-id="ce1d1-113">Reboot the computer, and log into OneDrive.</span></span>