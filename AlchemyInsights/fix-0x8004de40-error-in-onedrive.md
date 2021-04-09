---
title: Επιδιόρθωση 0x8004de40 σφάλματος στο OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649748"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="85223-102">Επιδιόρθωση 0x8004de40 σφάλματος στο OneDrive</span><span class="sxs-lookup"><span data-stu-id="85223-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="85223-103">Εάν χρησιμοποιείτε Windows 7 και λάβετε αυτό το σφάλμα, ενημερώστε το για να ενεργοποιήσετε τα [TLS 1.1 και TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)ως προεπιλεγμένα πρωτόκολλα ασφαλείας στο WinHTTP στα Windows.</span><span class="sxs-lookup"><span data-stu-id="85223-103">If you're running Windows 7 and receive this error, [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

<span data-ttu-id="85223-104">Εάν χρησιμοποιείτε Windows 10 και λάβετε ένα μήνυμα σφάλματος 0x8004de40 oneDrive:</span><span class="sxs-lookup"><span data-stu-id="85223-104">If you're running Windows 10, and you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="85223-105">Επανεκκινήστε τον υπολογιστή που επηρεάζεται ενώ είστε συνδεδεμένοι στον τομέα καταλόγου Acitve.</span><span class="sxs-lookup"><span data-stu-id="85223-105">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="85223-106">Εάν μια επανεκκίνηση δεν διορθώσει το πρόβλημα, αποσυνδεθείτε και επανασυνδεθείτε στη συσκευή σας από το Azure AD.</span><span class="sxs-lookup"><span data-stu-id="85223-106">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="85223-107">**Σημείωση:** Θα πρέπει να είστε στο εταιρικό σας δίκτυο κατά την εκτέλεση αυτών των βημάτων.</span><span class="sxs-lookup"><span data-stu-id="85223-107">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="85223-108">Μην εκτελείτε αυτά τα βήματα όταν δεν είστε συνδεδεμένοι στην εταιρική υποδομή σας (για παράδειγμα, ενώ ταξιδεύετε).</span><span class="sxs-lookup"><span data-stu-id="85223-108">Don't perform these steps when you aren't connected to your corporate infrastructure (for example, while traveling).</span></span> 

1. <span data-ttu-id="85223-109">Ανοίξτε μια αναβαθμισμένη γραμμή εντολών επιλέγοντας "Έναρξη", κάντε δεξί κλικ στη γραμμή **εντολών και,** στη συνέχεια, επιλέξτε **"Εκτέλεση ως διαχειριστής".**</span><span class="sxs-lookup"><span data-stu-id="85223-109">Open an elevated command prompt by selecting **Start**, right-click **Command Prompt**, and then select **Run as administrator**.</span></span>

1. <span data-ttu-id="85223-110">Πληκτρολογήστε *dsregcmd /leave και πατήστε* το **πλήκτρο Enter.**</span><span class="sxs-lookup"><span data-stu-id="85223-110">Type *dsregcmd /leave* and press **Enter**.</span></span>

1. <span data-ttu-id="85223-111">Όταν ολοκληρωθεί, πληκτρολογήστε *dsregcmd /join και πατήστε* το **πλήκτρο Enter.**</span><span class="sxs-lookup"><span data-stu-id="85223-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>

1. <span data-ttu-id="85223-112">Όταν ολοκληρωθεί, κλείστε τη γραμμή εντολών.</span><span class="sxs-lookup"><span data-stu-id="85223-112">When complete, close the command prompt.</span></span>

1. <span data-ttu-id="85223-113">Επανεκκινήστε τον υπολογιστή και συνδεθείτε στο OneDrive.</span><span class="sxs-lookup"><span data-stu-id="85223-113">Reboot the computer, and log into OneDrive.</span></span>