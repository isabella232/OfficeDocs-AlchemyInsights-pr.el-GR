---
title: 'Ρόλοι RBAC '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "7265"
ms.openlocfilehash: 7c4c9d1a76f395dfb2f831d555199b76c354ca57
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583545"
---
# <a name="rbac-rules"></a><span data-ttu-id="e9eb9-102">Κανόνες RBAC</span><span class="sxs-lookup"><span data-stu-id="e9eb9-102">RBAC rules</span></span>

<span data-ttu-id="e9eb9-103">Εάν λάβετε το σφάλμα δικαιωμάτων:</span><span class="sxs-lookup"><span data-stu-id="e9eb9-103">If you get the permission error:</span></span> 

- <span data-ttu-id="e9eb9-104">**Το πρόγραμμα-πελάτης με αναγνωριστικό αντικειμένου δεν έχει εξουσιοδότηση για την εκτέλεση ενέργειας μέσω του εύρους (Κωδικός: AuthorizationFailed)**: όταν προσπαθείτε να δημιουργήσετε έναν πόρο, βεβαιωθείτε ότι είστε συνδεδεμένοι με ένα χρήστη στον οποίο έχει εκχωρηθεί ένας ρόλος που έχει δικαίωμα εγγραφής στον πόρο στο επιλεγμένο πεδίο.</span><span class="sxs-lookup"><span data-stu-id="e9eb9-104">**The client with object id does not have authorization to perform action over scope (code: AuthorizationFailed)**: when you try to create a resource, check that you are currently signed in with a user that is assigned a role that has write permission to the resource at the selected scope.</span></span> <span data-ttu-id="e9eb9-105">Για παράδειγμα, για τη διαχείριση εικονικών μηχανημάτων σε μια ομάδα πόρων, θα πρέπει να έχετε το ρόλο " [συνεργάτης εικονικής μηχανής](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) " στην ομάδα πόρων (ή το γονικό πεδίο).</span><span class="sxs-lookup"><span data-stu-id="e9eb9-105">For example, to manage virtual machines in a resource group, you should have the [Virtual Machine Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) role on the resource group (or parent scope).</span></span> <span data-ttu-id="e9eb9-106">Για μια λίστα με τα δικαιώματα για κάθε ενσωματωμένο ρόλο, ανατρέξτε στο θέμα [ενσωματωμένοι ρόλοι για τους πόρους Azure](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="e9eb9-106">For a list of the permissions for each built-in role, see [Built-in roles for Azure resources](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
- <span data-ttu-id="e9eb9-107">**Δεν έχετε δικαιώματα για να δημιουργήσετε μια αίτηση υποστήριξης**: όταν προσπαθείτε να δημιουργήσετε ή να ενημερώσετε ένα δελτίο υποστήριξης, βεβαιωθείτε ότι έχετε εισέλθει τη συγκεκριμένη στιγμή με ένα χρήστη στον οποίο έχει εκχωρηθεί ένας ρόλος που έχει το δικαίωμα Microsoft. Support/supportTickets/write, όπως ο [συνεργάτης αίτησης υποστήριξης](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span><span class="sxs-lookup"><span data-stu-id="e9eb9-107">**You don't have permission to create a support request**: when you try to create or update a support ticket, check that you are currently signed in with a user that is assigned a role that has the Microsoft.Support/supportTickets/write permission, such as [Support Request Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span></span>
- <span data-ttu-id="e9eb9-108">**Δεν είναι δυνατή η δημιουργία περισσότερων αναθέσεων ρόλων (Κωδικός: RoleAssignmentLimitExceeded)**: όταν προσπαθείτε να εκχωρήσετε ένα ρόλο, προσπαθήστε να μειώσετε τον αριθμό των αναθέσεων ρόλων, αντιστοιχίζοντας ρόλους σε ομάδες αντ ' αυτού.</span><span class="sxs-lookup"><span data-stu-id="e9eb9-108">**No more role assignments can be created (code: RoleAssignmentLimitExceeded)**: when you try to assign a role, try to reduce the number of role assignments by assigning roles to groups instead.</span></span> <span data-ttu-id="e9eb9-109">Το Azure υποστηρίζει έως και **2000** αντιστοιχίσεις ρόλων ανά συνδρομή.</span><span class="sxs-lookup"><span data-stu-id="e9eb9-109">Azure supports up to **2000** role assignments per subscription.</span></span>

<span data-ttu-id="e9eb9-110">Για περισσότερες λεπτομέρειες σχετικά με τους ρόλους του Azure RBAC, ανατρέξτε στο θέμα [ρόλοι του Azure RBAC](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="e9eb9-110">For more details on Azure RBAC roles, see [Azure RBAC roles](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
