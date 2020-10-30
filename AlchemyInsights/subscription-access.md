---
title: Πρόσβαση σε συνδρομή
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003799"
- "6805"
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807432"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>Δεν είναι δυνατή η είσοδος στο Azure λόγω προβλημάτων του προγράμματος περιήγησης (το πρόγραμμα περιήγησης σταματά να ανταποκρίνεται, συνεχίζει να περιστρέφεται, δεν φορτώνεται, κ. λπ.)

Ενδέχεται να επηρεαστείτε από μια διακοπή ρεύματος. Παρακαλούμε ελέγξτε για να δείτε εάν υπάρχει συνεχιζόμενη διακοπή ρεύματος: [κατάσταση εύρυθμης λειτουργίας Azure](https://status.azure.com/status/history/).

Μπορείτε να αποσυνδεθείτε από όλες τις ενεργές περιόδους λειτουργίας Azure. Ξεκινήστε μια κατάσταση λειτουργίας in-Private ή ινκόγκνιτο του προγράμματος περιήγησής σας στο Web.

Θα μπορούσατε επίσης να δοκιμάσετε να ανανεώσετε το πρόγραμμα περιήγησης, να χρησιμοποιήσετε ένα άλλο πρόγραμμα περιήγησης, να διαγράψετε τα cookies cache αν δεν λειτουργεί.

Μάθετε περισσότερα: [αντιμετώπιση ζητημάτων εισόδου](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**Δεν είναι δυνατή η πρόσβαση σε συνδρομές**

Στην [πύλη Azure](https://portal.azure.com/), βεβαιωθείτε ότι έχει επιλεγεί ο σωστός Κατάλογος Azure από το λογαριασμό στην επάνω δεξιά γωνία.

Στο [Κέντρο λογαριασμού Azure](https://account.windowsazure.com/Subscriptions), βεβαιωθείτε ότι ο λογαριασμός που χρησιμοποιείται είναι ο διαχειριστής του λογαριασμού.

Μάθετε περισσότερα: [Αντιμετώπιση προβλημάτων χωρίς εύρεση συνδρομών](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**Δεν είναι δυνατή η πρόσβαση στο ιστορικό χρεώσεων**

Ο διαχειριστής του λογαριασμού πρέπει να βεβαιωθεί ότι ο χρήστης που έχει πρόσβαση στις πληροφορίες χρέωσης προστίθεται στο Azure Active Directory ως χρήστης επισκέπτη: [Προσθήκη ή διαγραφή νέου χρήστη](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

Στη συνέχεια, ο χρήστης πρέπει να αποκτήσει έναν ρόλο καθολικού διαχειριστή: [εκχώρηση ρόλου στους χρήστες](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Δημοσιεύστε αυτό το μήνυμα, ο χρήστης μπορεί να αποκτήσει πρόσβαση χρέωσης χρησιμοποιώντας τις πολιτικές RBAC: [εκχωρήστε πρόσβαση σε χρεώσεις](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).

**Προτεινόμενα έγγραφα**

-   [Δεν μπορώ να συνδεθώ για τη διαχείριση της συνδρομής μου στο Azure](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)