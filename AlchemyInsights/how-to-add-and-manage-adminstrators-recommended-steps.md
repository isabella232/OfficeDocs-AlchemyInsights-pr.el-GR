---
title: Πώς μπορείτε να προσθέσετε και να διαχειριστείτε διαχειριστές-Προτεινόμενα βήματα
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
ms.openlocfilehash: ed3aa5defabdd4f505ee4f74570023d990910dcb
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755835"
---
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a>Πώς μπορείτε να προσθέσετε και να διαχειριστείτε διαχειριστές-Προτεινόμενα βήματα

Με βάση την περιγραφή του ζητήματος, βρήκαμε μια λύση για εσάς. Οι περισσότεροι πελάτες μπόρεσαν να επιλύσουν το ζήτημά τους μόνοι τους, αφού ακολούθησαν την τεκμηρίωσή τους.

**Επεξεργασία του διαχειριστή συνδρομής ή του διαχειριστή**

- Ο διαχειριστής του λογαριασμού μπορεί να επεξεργαστεί και τους δύο ρόλους, ενώ ο διαχειριστής της συνδρομής μπορεί να αλλάξει μόνο τους διαχειριστές στην [πύλη Azure](https://ms.portal.azure.com/#home).
- [Προσθήκη ή αλλαγή των διαχειριστών συνδρομής Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

**Ενημέρωση του διαχειριστή συνδρομής ή του Co-Administrator για εσωτερικές συνδρομές (ΑΈΡΗΔες)**

Ο διαχειριστής της υπηρεσίας ή ο διαχειριστής μπορεί να εξυπηρετήσει αυτή την ενέργεια, χρησιμοποιώντας τα παρακάτω βήματα:

1. Συνδεθείτε στην [πύλη Azure](https://ms.portal.azure.com/#home) και κάντε κλικ στην επιλογή **Διαχείριση κόστους + χρέωση** στην αριστερή λάμα.
2. Κάντε κλικ στο στοιχείο γραμμή με τη συνδρομή σας. Αυτό ανοίγει την επισκόπηση για τη συνδρομή σας.
3. Στη λεπίδα **συνδρομής** , κάντε κλικ στην επιλογή **Ιδιότητες**. 
4. Κάντε κλικ στο κουμπί **διαχειριστής υπηρεσίας** .
5. Πληκτρολογήστε το μήνυμα ηλεκτρονικού ταχυδρομείου του χρήστη τον οποίο θέλετε να θέσετε ως διαχειριστή υπηρεσίας και κάντε κλικ στο κουμπί **OK**.

**Προσθήκη/Αλλαγή/Κατάργηση από κοινού διαχειριστή**

1. Συνδεθείτε στην [πύλη Azure](https://ms.portal.azure.com/#home) ως διαχειριστής υπηρεσίας.
2. Ανοίξτε τις [συνδρομές](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) και επιλέξτε μια συνδρομή. (Το διαχειριστές μπορεί να εκχωρηθεί μόνο στην εμβέλεια της συνδρομής.)
3. Περιήγηση στους κλασικούς διαχειριστές του **στοιχείου ελέγχου πρόσβασης (IAM)**  >    >  **Προσθήκη** του στοιχείου "  >  **Προσθήκη διαχειριστή** " για να ανοίξετε το τμήμα παραθύρου " **Προσθήκη** από κοινού διαχείρισης" (εάν η επιλογή "Προσθήκη διαχειριστή" είναι απενεργοποιημένη, υποδηλώνει ότι δεν έχετε δικαιώματα).
4. Επιλέξτε το χρήστη τον οποίο θέλετε να προσθέσετε και κάντε κλικ στην επιλογή **Προσθήκη**.

**Μάθε περισσότερα:**
- [Προσθήκη κοινού διαχειριστή](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Κατάργηση κοινού διαχειριστή](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Αλλαγή του διαχειριστή υπηρεσίας](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Προβολή του διαχειριστή λογαριασμού](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Διαχείριση της Access με χρήση του RBAC και του Azure Portal](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

**Προσθήκη/Διαγραφή χρηστών με χρήση του Azure Active Directory (AD)**

Μπορείτε να προσθέσετε νέους χρήστες ή να διαγράψετε υπάρχοντες χρήστες από τον οργανισμό Azure Active Directory (Azure AD):

1. Για να προσθέσετε έναν νέο χρήστη, συνδεθείτε στην [πύλη Azure](https://ms.portal.azure.com/#home) ως διαχειριστής χρήστη για τον οργανισμό.
2. Επιλέξτε **Azure Active Directory**, επιλέξτε **χρήστες** και, στη συνέχεια, κάντε κλικ στην επιλογή **νέος χρήστης**.
3. Στη σελίδα **χρήστη** , συμπληρώστε τις απαιτούμενες πληροφορίες. Κάντε κλικ στην επιλογή **Δημιουργία**. Ο χρήστης δημιουργείται και προστίθεται στον μισθωτή σας Azure AD.

**ΜΑΘΕΤΕ ΠΕΡΙΣΣΟΤΕΡΑ**:

- [Προσθήκη νέου χρήστη](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Διαγραφή χρήστη](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Προσθήκη ή ενημέρωση των πληροφοριών προφίλ ενός χρήστη με χρήση του Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

**Προτεινόμενα έγγραφα**

- [Τι είναι ο έλεγχος πρόσβασης βάσει ρόλων (RBAC);](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [Κατανόηση των διαφορετικών ρόλων στο Azure](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [Δικαιώματα ρόλου διαχειριστή στο Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [Πρόγραμμα εκμάθησης: εκχώρηση πρόσβασης για ένα χρήστη με χρήση του RBAC και της πύλης Azure](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [Αντιμετώπιση προβλημάτων του RBAC στο Azure](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [Οργάνωση των πόρων σας με τις ομάδες διαχείρισης του Azure](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [Πώς μπορείτε να ζητήσετε αντίγραφο του τιμολογίου Azure μέσω ηλεκτρονικού ταχυδρομείου](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [Πώς μπορείτε να προσθέσετε, να ενημερώσετε ή να καταργήσετε μια πιστωτική ή χρεωστική κάρτα από το Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [Διαχείριση (επανενεργοποίηση/ακύρωση/αλλαγή) συνδρομής](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



