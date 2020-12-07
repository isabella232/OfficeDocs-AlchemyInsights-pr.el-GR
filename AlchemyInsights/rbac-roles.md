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
# <a name="rbac-rules"></a>Κανόνες RBAC

Εάν λάβετε το σφάλμα δικαιωμάτων: 

- **Το πρόγραμμα-πελάτης με αναγνωριστικό αντικειμένου δεν έχει εξουσιοδότηση για την εκτέλεση ενέργειας μέσω του εύρους (Κωδικός: AuthorizationFailed)**: όταν προσπαθείτε να δημιουργήσετε έναν πόρο, βεβαιωθείτε ότι είστε συνδεδεμένοι με ένα χρήστη στον οποίο έχει εκχωρηθεί ένας ρόλος που έχει δικαίωμα εγγραφής στον πόρο στο επιλεγμένο πεδίο. Για παράδειγμα, για τη διαχείριση εικονικών μηχανημάτων σε μια ομάδα πόρων, θα πρέπει να έχετε το ρόλο " [συνεργάτης εικονικής μηχανής](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) " στην ομάδα πόρων (ή το γονικό πεδίο). Για μια λίστα με τα δικαιώματα για κάθε ενσωματωμένο ρόλο, ανατρέξτε στο θέμα [ενσωματωμένοι ρόλοι για τους πόρους Azure](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).
- **Δεν έχετε δικαιώματα για να δημιουργήσετε μια αίτηση υποστήριξης**: όταν προσπαθείτε να δημιουργήσετε ή να ενημερώσετε ένα δελτίο υποστήριξης, βεβαιωθείτε ότι έχετε εισέλθει τη συγκεκριμένη στιγμή με ένα χρήστη στον οποίο έχει εκχωρηθεί ένας ρόλος που έχει το δικαίωμα Microsoft. Support/supportTickets/write, όπως ο [συνεργάτης αίτησης υποστήριξης](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).
- **Δεν είναι δυνατή η δημιουργία περισσότερων αναθέσεων ρόλων (Κωδικός: RoleAssignmentLimitExceeded)**: όταν προσπαθείτε να εκχωρήσετε ένα ρόλο, προσπαθήστε να μειώσετε τον αριθμό των αναθέσεων ρόλων, αντιστοιχίζοντας ρόλους σε ομάδες αντ ' αυτού. Το Azure υποστηρίζει έως και **2000** αντιστοιχίσεις ρόλων ανά συνδρομή.

Για περισσότερες λεπτομέρειες σχετικά με τους ρόλους του Azure RBAC, ανατρέξτε στο θέμα [ρόλοι του Azure RBAC](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).
