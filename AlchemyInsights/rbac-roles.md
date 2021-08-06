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
ms.openlocfilehash: 1faa9f69942d39b8d78c8f3e1316f93b52eeede6408dfabc89d0f7fe38b86fb3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923131"
---
# <a name="rbac-rules"></a>Κανόνες RBAC

Εάν εμφανιστεί το σφάλμα δικαιωμάτων: 

- Το πρόγραμμα-πελάτης με αναγνωριστικό αντικειμένου δεν έχει εξουσιοδότηση για την εκτέλεση ενεργειών μέσω εμβέλειας **(κωδικός: AuthorizationFailed)**: όταν προσπαθείτε να δημιουργήσετε έναν πόρο, ελέγξτε ότι έχετε πραγματοποιήσει αυτήν τη στιγμή εισέλθει με ένα χρήστη στον οποίο έχει εκχωρηθεί ένας ρόλος που έχει δικαίωμα εγγραφής στον πόρο στο επιλεγμένο εύρος. Για παράδειγμα, για να διαχειριστείτε εικονικές μηχανές σε μια ομάδα πόρων, θα πρέπει να έχετε το ρόλο [συμβολής](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) εικονικής μηχανής στην ομάδα πόρων (ή στο γονικό εύρος). Για μια λίστα με τα δικαιώματα για κάθε ενσωματωμένο ρόλο, ανατρέξτε στο θέμα [Ενσωματωμένοι ρόλοι για τους πόρους Azure.](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support)
- **Δεν έχετε** δικαίωμα να δημιουργήσετε ένα αίτημα υποστήριξης: όταν προσπαθείτε να δημιουργήσετε ή να ενημερώσετε ένα δελτίο υποστήριξης, ελέγξτε ότι έχετε εισέλθει αυτήν τη στιγμή με ένα χρήστη στον οποίο έχει εκχωρηθεί ένας ρόλος που έχει το δικαίωμα Microsoft.Support/supportTickets/write, όπως "Συνεργάτης αίτησης [υποστήριξης".](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor)
- Δεν είναι δυνατό να δημιουργηθούν άλλες αναθέσεις ρόλων **(κώδικας: RoleAssignmentLimitExceed)**: όταν προσπαθείτε να αναθέσετε ένα ρόλο, προσπαθήστε να μειώσετε τον αριθμό των αναθέσεων ρόλων εκχωρώντας ρόλους σε ομάδες. Το Azure υποστηρίζει έως **2.000 αναθέσεις** ρόλων ανά συνδρομή.

Για περισσότερες λεπτομέρειες σχετικά με τους ρόλους του Azure RBAC, ανατρέξτε [στο θέμα Ρόλοι Azure RBAC.](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support)
