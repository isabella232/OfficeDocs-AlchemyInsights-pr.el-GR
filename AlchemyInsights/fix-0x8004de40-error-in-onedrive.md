---
title: Επιδιόρθωση του σφάλματος 0x8004de40 στο OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: b9bd6dff48f78063e3d47f5fe2f834f59eb9868a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745130"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="6f692-102">Επιδιόρθωση του σφάλματος 0x8004de40 στο OneDrive</span><span class="sxs-lookup"><span data-stu-id="6f692-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="6f692-103">Εάν εμφανιστεί ένα σφάλμα 0x8004de40 με το OneDrive:</span><span class="sxs-lookup"><span data-stu-id="6f692-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="6f692-104">Επανεκκινήστε τον υπολογιστή που επηρεάζεται ενώ είστε συνδεδεμένοι με τον τομέα καταλόγου του acitve.</span><span class="sxs-lookup"><span data-stu-id="6f692-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="6f692-105">Εάν η επανεκκίνηση δεν διορθώσει το πρόβλημα, αποσυνδεθείτε και επανσυνδεθείτε στη συσκευή σας από το Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6f692-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="6f692-106">**Σημείωση**: θα πρέπει να βρίσκεστε στο εταιρικό σας δίκτυο κατά την εκτέλεση αυτών των βημάτων.</span><span class="sxs-lookup"><span data-stu-id="6f692-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="6f692-107">Μην εκτελείτε αυτά τα βήματα όταν δεν μπορείτε να συνδεθείτε με την εταιρική σας υποδομή (για παράδειγμα, ενώ ταξιδεύετε).</span><span class="sxs-lookup"><span data-stu-id="6f692-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="6f692-108">Ανοίξτε μια γραμμή εντολών με αυξημένα δικαιώματα.</span><span class="sxs-lookup"><span data-stu-id="6f692-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="6f692-109">Για να ανοίξετε μια γραμμή εντολών με αυξημένα δικαιώματα, κάντε κλικ στην επιλογή- **Έναρξη**, κάντε δεξί κλικ στη γραμμή **εντολών**και, στη συνέχεια, κάντε κλικ στην επιλογή **Εκτέλεση ως διαχειριστής**.</span><span class="sxs-lookup"><span data-stu-id="6f692-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="6f692-110">Πληκτρολογήστε *dsregcmd/Leave* και πατήστε το πλήκτρο **ENTER**.</span><span class="sxs-lookup"><span data-stu-id="6f692-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="6f692-111">Όταν ολοκληρωθεί, πληκτρολογήστε *dsregcmd/Join* και πατήστε το πλήκτρο **ENTER**.</span><span class="sxs-lookup"><span data-stu-id="6f692-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="6f692-112">Όταν ολοκληρωθεί, κλείστε τη γραμμή εντολών.</span><span class="sxs-lookup"><span data-stu-id="6f692-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="6f692-113">Επανεκκινήστε τον υπολογιστή και συνδεθείτε στο OneDrive.</span><span class="sxs-lookup"><span data-stu-id="6f692-113">Reboot the computer, and log into OneDrive.</span></span>