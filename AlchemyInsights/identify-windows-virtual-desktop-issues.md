---
title: Προσδιορισμός προβλημάτων εικονικής επιφάνειας εργασίας των Windows
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O364
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 1e55d9d579c389dfe731f887a2a08c6234de2787
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595629"
---
# <a name="identify-windows-virtual-desktop-issues"></a><span data-ttu-id="ce154-102">Προσδιορισμός προβλημάτων εικονικής επιφάνειας εργασίας των Windows</span><span class="sxs-lookup"><span data-stu-id="ce154-102">Identify Windows Virtual Desktop issues</span></span>

<span data-ttu-id="ce154-103">Τα Διαγνωστικά εικονικής επιφάνειας εργασίας των Windows χρησιμοποιούν μόνο ένα cmdlet του PowerShell, αλλά περιέχουν πολλές προαιρετικές παραμέτρους για να σας βοηθήσουν να περιορίσετε και να απομονώσετε προβλήματα.</span><span class="sxs-lookup"><span data-stu-id="ce154-103">Windows Virtual Desktop Diagnostics uses just one PowerShell cmdlet but contains many optional parameters to help narrow down and isolate issues.</span></span> <span data-ttu-id="ce154-104">Για να ξεκινήσετε:</span><span class="sxs-lookup"><span data-stu-id="ce154-104">To get started:</span></span> 

1. <span data-ttu-id="ce154-105">Κάντε λήψη και εισαγωγή της λειτουργικής μονάδας PowerShell εικονικής επιφάνειας εργασίας των Windows.</span><span class="sxs-lookup"><span data-stu-id="ce154-105">Download and import the Windows Virtual Desktop PowerShell module.</span></span> <span data-ttu-id="ce154-106">Για λεπτομέρειες, [ανατρέξτε στα Cmdlet εικονικής επιφάνειας εργασίας των Windows για το Windows PowerShell.](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview)</span><span class="sxs-lookup"><span data-stu-id="ce154-106">For details, see [Windows Virtual Desktop Cmdlets for Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).</span></span>

1. <span data-ttu-id="ce154-107">Εκτελέστε το ακόλουθο cmdlet για να εισέλθετε στο λογαριασμό σας:</span><span class="sxs-lookup"><span data-stu-id="ce154-107">Run the following cmdlet to sign in to your account:</span></span>
    
    <span data-ttu-id="ce154-108">Παράδειγμα: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span><span class="sxs-lookup"><span data-stu-id="ce154-108">Example: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span></span>

<span data-ttu-id="ce154-109">**ΣΗΜΕΙΩΣΗ:** Όλα τα ερωτήματα που χρησιμοποιούν το PowerShell πρέπει να περιλαμβάνουν τις παραμέτρους -Όνομα χρήστη ή -ActivityID.</span><span class="sxs-lookup"><span data-stu-id="ce154-109">**NOTE:** All queries using PowerShell must include either the -UserName or -ActivityID parameters.</span></span> <span data-ttu-id="ce154-110">Για δυνατότητες παρακολούθησης, ανατρέξτε στο θέμα "Χρήση [ανάλυσης καταγραφής" για τη δυνατότητα διαγνωστικών.](https://go.microsoft.com/fwlink/?linkid=2126847)</span><span class="sxs-lookup"><span data-stu-id="ce154-110">For monitoring capabilities, see Use [Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2126847).</span></span>

<span data-ttu-id="ce154-111">Για να φιλτράρετε τις διαγνωστικές δραστηριότητες κατά χρήστη, εκτελέστε το ακόλουθο cmdlet:</span><span class="sxs-lookup"><span data-stu-id="ce154-111">To filter diagnostic activities by user, run the following cmdlet:</span></span>

<span data-ttu-id="ce154-112">Παράδειγμα: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span><span class="sxs-lookup"><span data-stu-id="ce154-112">Example: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span></span>

<span data-ttu-id="ce154-113">Υπάρχει μια λίστα φίλτρων που μπορείτε να εκτελέσετε για τη διάγνωση προβλημάτων.</span><span class="sxs-lookup"><span data-stu-id="ce154-113">There is a list of filters you can run to diagnose issues.</span></span> <span data-ttu-id="ce154-114">Για να μάθετε περισσότερα σχετικά με τη διάγνωση προβλημάτων, ανατρέξτε στο θέμα [Αναγνώριση και διάγνωση ζητημάτων εικονικής επιφάνειας εργασίας των Windows.](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell)</span><span class="sxs-lookup"><span data-stu-id="ce154-114">To learn more about diagnosing issues, see [Identify and diagnose Windows Virtual Desktop issues](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell).</span></span>

<span data-ttu-id="ce154-115">Για να μάθετε περισσότερα σχετικά με τα συνηθισμένα σφάλματα, ανατρέξτε στο θέμα [Κοινά σφάλματα senarios.](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios)</span><span class="sxs-lookup"><span data-stu-id="ce154-115">To learn more about common errors, see [Common errors senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).</span></span>
