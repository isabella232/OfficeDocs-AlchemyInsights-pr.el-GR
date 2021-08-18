---
title: Τρόπος προσθήκης και διαχείρισης διαχειριστών - προτεινόμενα βήματα
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/07/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7194"
ms.openlocfilehash: 48a06fde215e007b6b81b32ab751ca8e4bba522d
ms.sourcegitcommit: 46e24d65cffd37b6988447c6738b3315303bbe13
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58339032"
---
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a>Τρόπος προσθήκης και διαχείρισης διαχειριστών - προτεινόμενα βήματα

Με βάση την περιγραφή του προβλήματος, έχουμε βρει μια λύση για εσάς. Οι περισσότεροι πελάτες είχαν τη δυνατότητα να επιλύσουν το πρόβλημά τους μόνοι τους μετά την τεκμηρίωση.

**Επεξεργασία του διαχειριστή συνδρομής ή του διαχειριστή από συνεργασία**

- Ο διαχειριστής λογαριασμού μπορεί να επεξεργαστεί και τους δύο ρόλους, ενώ ο διαχειριστής συνδρομής μπορεί να αλλάξει μόνο τους συν-διαχειριστές [στην πύλη Azure.](https://ms.portal.azure.com/#home)
- [Προσθήκη ή αλλαγή διαχειριστών συνδρομής Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

**Ενημέρωση του διαχειριστή συνδρομής ή Co-Administrator για εσωτερικές συνδρομές (AIRS)**

Ο διαχειριστής της υπηρεσίας ή ο διαχειριστής από τον ίδιο τον διαχειριστή μπορεί να κάνει αυτο-εξυπηρέτηση αυτής της ενέργειας, ακολουθώντας τα παρακάτω βήματα:

1. Συνδεθείτε στην πύλη [Azure και κάντε κλικ](https://ms.portal.azure.com/#home) στην επιλογή Διαχείριση κόστους + **Χρέωση** στην αριστερή λάμα.
2. Κάντε κλικ στο στοιχείο γραμμής με τη συνδρομή σας. Με αυτόν τον τρόπο ανοίγει η Επισκόπηση για τη συνδρομή σας.
3. Στη blade **της συνδρομής,** κάντε κλικ στην επιλογή **"Ιδιότητες".** 
4. Κάντε κλικ **στο κουμπί "Διαχείριση υπηρεσίας".**
5. Πληκτρολογήστε το μήνυμα ηλεκτρονικού ταχυδρομείου του χρήστη τον οποίο θέλετε να ορίσετε ως διαχειριστή υπηρεσίας και κάντε κλικ στο **κουμπί OK.**

**Προσθήκη/Αλλαγή/Κατάργηση διαχειριστή από το co-administrator**

1. Συνδεθείτε στην πύλη [Azure ως](https://ms.portal.azure.com/#home) διαχειριστής υπηρεσίας.
2. Ανοίξτε [τις Συνδρομές](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) και επιλέξτε μια συνδρομή. (Οι συν-διαχειριστές μπορούν να εκχωρούνται μόνο στο εύρος της συνδρομής.)
3. Μεταβείτε στην κλασική επιλογή "Έλεγχος **πρόσβασης" (IAM)**"Προσθήκη συν-διαχειριστή" για να ανοίξετε το παράθυρο "Προσθήκη  >    >    >   **συν-διαχειριστή"** (Εάν η επιλογή "Προσθήκη συν-διαχειριστή" είναι απενεργοποιημένη, αυτό σημαίνει ότι δεν έχετε δικαιώματα).
4. Επιλέξτε το χρήστη που θέλετε να προσθέσετε και κάντε κλικ στην επιλογή **"Προσθήκη".**

**Μάθε περισσότερα:**
- [Προσθήκη συν-διαχειριστή](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Κατάργηση διαχειριστή από συνεργασία](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Αλλαγή του διαχειριστή υπηρεσίας](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Προβολή του διαχειριστή λογαριασμού](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Διαχείριση πρόσβασης με χρήση της πύλης RBAC και του Azure](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

**Προσθήκη/διαγραφή χρηστών με χρήση Azure Active Directory (AD)**

Μπορείτε να προσθέσετε νέους χρήστες ή να διαγράψετε υπάρχοντες χρήστες από τον οργανισμό Azure Active Directory (Azure AD):

1. Για να προσθέσετε έναν νέο χρήστη, συνδεθείτε στην [πύλη Azure](https://ms.portal.azure.com/#home) ως διαχειριστής χρήστη για τον οργανισμό.
2. Επιλέξτε **Azure Active Directory, επιλέξτε**"Χρήστες" **και, στη** συνέχεια, κάντε κλικ στην επιλογή **"Νέος χρήστης".**
3. Στη σελίδα **"Χρήστης",** συμπληρώστε τις απαιτούμενες πληροφορίες. Κάντε κλικ **στην επιλογή "Δημιουργία".** Ο χρήστης δημιουργείται και προστίθεται στο μισθωτή azure AD.

**Μάθετε περισσότερα:**

- [Προσθήκη νέου χρήστη](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Διαγραφή χρήστη](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Προσθήκη ή ενημέρωση πληροφοριών προφίλ χρήστη με χρήση Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

**Προτεινόμενα έγγραφα**

- [Τι είναι ο έλεγχος πρόσβασης βάσει ρόλων (RBAC);](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [Κατανόηση των διαφορετικών ρόλων στο Azure](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [Δικαιώματα ρόλων διαχειριστή στο Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [Πρόγραμμα εκμάθησης: Εκχώρηση πρόσβασης για ένα χρήστη που χρησιμοποιεί το RBAC και την πύλη Azure](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [Αντιμετώπιση προβλημάτων RBAC στο Azure](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [Οργάνωση των πόρων σας με ομάδες διαχείρισης Azure](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [Πώς μπορείτε να ζητήσετε αντίγραφο του τιμολογίου Azure μέσω ηλεκτρονικού ταχυδρομείου](https://azure.microsoft.com/blog/azure-email-invoices/)
- [Τρόπος προσθήκης, ενημέρωσης ή κατάργησης πιστωτικής ή χρεωστικής κάρτας από το Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [Διαχείριση (Επανενεργοποίηση/Ακύρωση/Αλλαγή) συνδρομής](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



