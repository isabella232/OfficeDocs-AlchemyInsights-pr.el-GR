---
title: Διορθώστε το σφάλμα 0x8004de40 στο OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: d436184bdc0e283db217ea734fb2c8e05f85b4e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525059"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="1137e-102">Διορθώστε το σφάλμα 0x8004de40 στο OneDrive</span><span class="sxs-lookup"><span data-stu-id="1137e-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="1137e-103">Εάν λαμβάνετε ένα μήνυμα λάθους 0x8004de40 με OneDrive:</span><span class="sxs-lookup"><span data-stu-id="1137e-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="1137e-104">Κάντε επανεκκίνηση του υπολογιστή που επηρεάζεται, ενώ είστε συνδεδεμένοι στον τομέα σας κατάλογο ενρεγό.</span><span class="sxs-lookup"><span data-stu-id="1137e-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="1137e-105">Εάν η επανεκκίνηση δεν διορθώσει το ζήτημα, απομονώστε και Επανασυνδέστε τη συσκευή σας από Azure AD.</span><span class="sxs-lookup"><span data-stu-id="1137e-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="1137e-106">**Σημείωση**: θα πρέπει να είναι στο εταιρικό σας δίκτυο, ενώ εκτελείτε αυτά τα βήματα.</span><span class="sxs-lookup"><span data-stu-id="1137e-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="1137e-107">Μην εκτελέσετε αυτά τα βήματα, όταν δεν μπορείτε να συνδεθείτε με την υποδομή της εταιρείας σας (για παράδειγμα, ενώ ταξιδεύετε).</span><span class="sxs-lookup"><span data-stu-id="1137e-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="1137e-108">Ανοίξτε μια γραμμή εντολών με αυξημένα δικαιώματα.</span><span class="sxs-lookup"><span data-stu-id="1137e-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="1137e-109">Για να ανοίξετε μια γραμμή εντολών με αυξημένα δικαιώματα, κάντε κλικ στην - **Έναρξη**, κάντε δεξιό κλικ σε **γραμμή εντολών**και, στη συνέχεια, κάντε κλικ στην εντολή **Εκτέλεση ως διαχειριστής**.</span><span class="sxs-lookup"><span data-stu-id="1137e-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="1137e-110">Πληκτρολογήστε *dsregcmd /leave* και πιέστε το πλήκτρο **Enter**.</span><span class="sxs-lookup"><span data-stu-id="1137e-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="1137e-111">Όταν ολοκληρωθεί η εγκατάσταση, πληκτρολογήστε *dsregcmd /join* και πιέστε το πλήκτρο **Enter**.</span><span class="sxs-lookup"><span data-stu-id="1137e-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="1137e-112">Όταν τελειώσετε, κλείστε τη γραμμή εντολών.</span><span class="sxs-lookup"><span data-stu-id="1137e-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="1137e-113">Ξεκινήστε πάλι τον υπολογιστή και συνδεθείτε στο OneDrive.</span><span class="sxs-lookup"><span data-stu-id="1137e-113">Reboot the computer, and log into OneDrive.</span></span>