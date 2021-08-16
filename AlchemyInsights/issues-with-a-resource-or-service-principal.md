---
title: Προβλήματα με έναν πόρο ή μια αρχή υπηρεσίας
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
ms.openlocfilehash: 52b9b2e950d66c2f4105b76c4e2c70ed51320e4a57eb0008c353a9587fcc6510
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028076"
---
# <a name="issues-with-a-resource-or-service-principal"></a>Προβλήματα με έναν πόρο ή μια αρχή υπηρεσίας

1. Εάν μόλις ξεκινάτε, τα κύρια αντικείμενα εφαρμογών και υπηρεσιών στο [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) περιγράφουν την καταχώρηση εφαρμογών, τα αντικείμενα εφαρμογών και τις κύριες αρχές υπηρεσιών στο Azure Active Directory: τι είναι, πώς χρησιμοποιούνται και πώς σχετίζονται μεταξύ τους. Παρουσιάζεται επίσης ένα παράδειγμα σεναρίου πολλών μισθωτών για να απεικονίσει τη σχέση μεταξύ του αντικειμένου εφαρμογής μιας εφαρμογής και των αντίστοιχων αντικειμένων κύριας υπηρεσίας.
2. Μπορείτε να μάθετε περισσότερα σχετικά με τη σχέση μεταξύ των εφαρμογών και των εντολών υπηρεσιών, διαβάζοντας [εφαρμογές και κύρια αντικείμενα υπηρεσιών στο Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)
3. [Τρόπος:](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) Χρησιμοποιήστε την πύλη για να δημιουργήσετε μια κύρια εφαρμογή και υπηρεσία Azure AD που μπορεί να αποκτήσει πρόσβαση σε πόρους που δείχνει πώς μπορείτε να δημιουργήσετε μια νέα εφαρμογή και κύρια υπηρεσία του Azure Active Directory (Azure AD) που μπορεί να χρησιμοποιηθεί με τον έλεγχο πρόσβασης βάσει ρόλων.
4. Με το [κύριο API της υπηρεσίας,](https://docs.microsoft.com/graph/api/resources/serviceprincipal)μπορείτε να διαχειρίζεστε μέσω προγραμματισμού παρουσίες εφαρμογών και να ελέγχετε τι μπορεί να κάνει μια εφαρμογή μέσα στο μισθωτή σας.
5. [Ο τύπος πόρου servicePrincipal παραθέτει](https://docs.microsoft.com/graph/api/resources/serviceprincipal) όλες τις ιδιότητες και τις μεθόδους για τον τύπο πόρου servicePrincipal.
6. [Οι διαφορές τύπου πόρων μεταξύ του Azure AD Graph και του Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) επισημαίνει τις διαφορές μεταξύ του Azure AD Graph και των πόρων Graph Microsoft. Εμφανίζει πόρους που έχουν διαφορετικά ονόματα ή δεν είναι διαθέσιμοι. Επισημαίνει επίσης πόρους που είναι διαθέσιμοι στην έκδοση beta του Microsoft Graph αλλά όχι στην έκδοση v1.0.

**Προβλήματα με τους χρήστες-επισκέπτες**

- [Γρήγορη εκκίνηση:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) Η προσθήκη χρηστών-επισκεπτών στον κατάλογο στην πύλη Azure σάς δείχνει πώς μπορείτε να προσθέσετε έναν νέο χρήστη-επισκέπτη στον κατάλογο Azure AD μέσω της πύλης Azure, να στείλετε μια πρόσκληση και να δείτε πώς μοιάζει η διαδικασία εξαργύρωσης πρόσκλησης του χρήστη-επισκέπτη.
- [Πρόγραμμα εκμάθησης: Η δημιουργία ροών χρηστών Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) σάς δείχνει πώς μπορείτε να δημιουργήσετε ορισμένες προτεινόμενες ροές χρηστών χρησιμοποιώντας την πύλη Azure. Εάν αναζητάτε πληροφορίες σχετικά με τον τρόπο ρύθμισης μιας ροής διαπιστευτηρίων κωδικού πρόσβασης κατόχου πόρου (ROPC) στην εφαρμογή σας, ανατρέξτε στο θέμα Ρύθμιση παραμέτρων της ροής διαπιστευτηρίων κωδικού πρόσβασης κατόχου πόρου στο Azure AD B2C.
