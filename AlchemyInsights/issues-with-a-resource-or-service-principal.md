---
title: Ζητήματα με μια κύρια υπηρεσία ή πόρο
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
- "9004336"
- "7741"
ms.openlocfilehash: 9c37ad8e4dfecdb59a37d767f8eb4a5d99be7fa1
ms.sourcegitcommit: d13f23fb7994871d4e0e6e3e43672a101bd779e8
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/28/2021
ms.locfileid: "50713663"
---
# <a name="issues-with-a-resource-or-service-principal"></a>Ζητήματα με μια κύρια υπηρεσία ή πόρο

1. Εάν μόλις ξεκινάτε, τα κύρια αντικείμενα εφαρμογών και υπηρεσιών στο [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) περιγράφουν την καταχώρηση εφαρμογών, τα αντικείμενα εφαρμογών και τις κύριες αρχές υπηρεσίας στο Azure Active Directory: τι είναι, πώς χρησιμοποιούνται και πώς σχετίζονται μεταξύ τους. Παρουσιάζεται επίσης ένα παράδειγμα σεναρίου πολλών μισθωτών για να απεικονίσει τη σχέση μεταξύ του αντικειμένου εφαρμογής μιας εφαρμογής και των αντίστοιχων αντικειμένων κύριας υπηρεσίας.
2. Μπορείτε να μάθετε περισσότερα σχετικά με τη σχέση μεταξύ εφαρμογών και εντολών υπηρεσίας, διαβάζοντας εφαρμογές και [αντικείμενα κύριας υπηρεσίας στο Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)
3. [Διαδικασία:](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) Χρησιμοποιήστε την πύλη για να δημιουργήσετε μια κύρια εφαρμογή και υπηρεσία του Azure AD που έχει πρόσβαση σε πόρους και σας δείχνει πώς μπορείτε να δημιουργήσετε μια νέα εφαρμογή και κύρια υπηρεσία του Azure Active Directory (Azure AD) που μπορεί να χρησιμοποιηθεί με το στοιχείο ελέγχου πρόσβασης βάσει ρόλων.
4. Με την [κύρια υπηρεσία API,](https://docs.microsoft.com/graph/api/resources/serviceprincipal)μπορείτε να διαχειρίζεστε με προγραμματισμού παρουσίες εφαρμογών και να ελέγχετε τι μπορεί να κάνει μια εφαρμογή στο μισθωτή σας.
5. [Ο τύπος πόρου servicePrincipal παραθέτει όλες](https://docs.microsoft.com/graph/api/resources/serviceprincipal) τις ιδιότητες και τις μεθόδους για τον τύπο πόρου servicePrincipal.
6. [Οι διαφορές τύπου πόρων μεταξύ του Azure AD Graph και του Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) επιδεικνύουν διαφορές μεταξύ του Azure AD Graph και των πόρων του Microsoft Graph. Εμφανίζει πόρους που έχουν διαφορετικά ονόματα ή δεν είναι διαθέσιμοι. Επισημαίνει επίσης πόρους που είναι διαθέσιμοι στην έκδοση beta του Microsoft Graph, αλλά όχι στην έκδοση v1.0.

**Προβλήματα με τους χρήστες-επισκέπτες**

- [Γρήγορη εκκίνηση:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) Η προσθήκη χρηστών-επισκεπτών στον κατάλογο στην πύλη Azure σάς δείχνει πώς μπορείτε να προσθέσετε έναν νέο χρήστη-επισκέπτη στον κατάλογο azure AD μέσω της πύλης Azure, να στείλετε μια πρόσκληση και να δείτε πώς μοιάζει η διαδικασία εξαργύρωσης προσκλήσεων του χρήστη-επισκέπτη.
- [Πρόγραμμα εκμάθησης: Η δημιουργία ροών χρηστών στο Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) σάς δείχνει πώς μπορείτε να δημιουργήσετε ορισμένες προτεινόμενες ροές χρηστών χρησιμοποιώντας την πύλη Azure. Εάν αναζητάτε πληροφορίες σχετικά με τον τρόπο ρύθμισης μιας ροής διαπιστευτηρίων κωδικού πρόσβασης κατόχου πόρου (ROPC) στην εφαρμογή σας, ανατρέξτε στο θέμα "Ρύθμιση παραμέτρων της ροής διαπιστευτηρίων κωδικού πρόσβασης κατόχου πόρου στο Azure AD B2C".
