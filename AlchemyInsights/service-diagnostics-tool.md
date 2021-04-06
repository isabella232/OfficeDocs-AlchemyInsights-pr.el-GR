---
title: Εργαλείο διαγνωστικών υπηρεσίας για την εικονική επιφάνεια εργασίας των Windows
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: dfa59c86508c8658c880f4f3f21a002524e909d1
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595630"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="b8f64-102">Εργαλείο διαγνωστικών υπηρεσίας για την εικονική επιφάνεια εργασίας των Windows</span><span class="sxs-lookup"><span data-stu-id="b8f64-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="b8f64-103">Η Εικονική επιφάνεια εργασίας των Windows (WVD) προσφέρει ένα διαγνωστικό εργαλείο που επιτρέπει στους διαχειριστές να εντοπίζουν σφάλματα μέσω ενός μόνο περιβάλλοντος εργασίας.</span><span class="sxs-lookup"><span data-stu-id="b8f64-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="b8f64-104">Αυτό το εργαλείο καταγράφει πληροφορίες που σχετίζονται με διαγνωστικά κάθε φορά που το WVD χρησιμοποιείται από κάποιον στον οποίο έχει εκχωρηθεί ένας ρόλος WVD.</span><span class="sxs-lookup"><span data-stu-id="b8f64-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="b8f64-105">Κάθε αρχείο καταγραφής περιέχει πληροφορίες σχετικά με το ρόλο WVD που εμπλέκεται στη δραστηριότητα, τα μηνύματα σφάλματος που εμφανίζονται κατά τη διάρκεια της περιόδου λειτουργίας και τις πληροφορίες σχετικά με το μισθωτή και το χρήστη.</span><span class="sxs-lookup"><span data-stu-id="b8f64-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="b8f64-106">Μπορείτε να ρυθμίσετε τις παραμέτρους του Azure Log Analytics για να καταγράψετε το αρχείο καταγραφής δραστηριότητας που δημιουργήθηκε από το εργαλείο διαγνωστικών, ακολουθώντας τα παρακάτω βήματα:</span><span class="sxs-lookup"><span data-stu-id="b8f64-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool by following these steps:</span></span>

1. <span data-ttu-id="b8f64-107">Δημιουργήστε ένα χώρο εργασίας ανάλυσης αρχείων καταγραφής με [την πύλη Azure](https://go.microsoft.com/fwlink/?linkid=2129500) ή το Azure [PowerShell.](https://go.microsoft.com/fwlink/?linkid=2129501)</span><span class="sxs-lookup"><span data-stu-id="b8f64-107">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>

1. <span data-ttu-id="b8f64-108">[Συνδέστε υπολογιστές Windows στο Azure Monitor.](https://go.microsoft.com/fwlink/?linkid=2129913)</span><span class="sxs-lookup"><span data-stu-id="b8f64-108">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="b8f64-109">Αποκτήστε το αναγνωριστικό χώρου εργασίας και το πρωτεύον κλειδί του χώρου εργασίας σας.</span><span class="sxs-lookup"><span data-stu-id="b8f64-109">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="b8f64-110">Ο οδηγός ρύθμισης χρειάζεται αυτές τις πληροφορίες για να ρυθμίσει σωστά τις παραμέτρους του παράγοντα και για να εξασφαλίσει ότι μπορεί να επικοινωνήσει με το Azure Monitor.</span><span class="sxs-lookup"><span data-stu-id="b8f64-110">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>

1. <span data-ttu-id="b8f64-111">[Προωθήτε δεδομένα διαγνωστικών στο χώρο εργασίας σας.](https://go.microsoft.com/fwlink/?linkid=2128284)</span><span class="sxs-lookup"><span data-stu-id="b8f64-111">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="b8f64-112">Μπορείτε να ωθήσετε τα δεδομένα διαγνωστικών από το μισθωτή WVD στην Ανάλυση καταγραφής για το χώρο εργασίας σας.</span><span class="sxs-lookup"><span data-stu-id="b8f64-112">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>

1. <span data-ttu-id="b8f64-113">[Προσδιορίστε και διαγνώστε](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) ζητήματα που είναι εσωτερικά ή εξωτερικά σε σχέση με το WVD.</span><span class="sxs-lookup"><span data-stu-id="b8f64-113">[Identify and diagnose](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) issues that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="b8f64-114">Για να μάθετε περισσότερα σχετικά με τη ρύθμιση παραμέτρων του εργαλείου διαγνωστικών υπηρεσίας για το WVD, ανατρέξτε στο θέμα "Χρήση ανάλυσης αρχείου καταγραφής" για τη δυνατότητα διαγνωστικών.</span><span class="sxs-lookup"><span data-stu-id="b8f64-114">To learn more about configuring the service diagnostics tool for WVD, see Use Log Analytics for the diagnostics feature.</span></span>