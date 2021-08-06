---
title: Πρόσβαση συνδρομής
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
ms.openlocfilehash: b138c05e87e70c18bb6528819a34f8a9501446d57dcf4dbac0734f70fbc3466b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53999240"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>Δεν είναι δυνατή η είσοδος στο Azure λόγω προβλημάτων του προγράμματος περιήγησης (Το πρόγραμμα περιήγησης σταματά να λειτουργεί, συνεχίζει να περιστρέφεται, δεν φορτώνει κ.λπ.)

Ενδέχεται να σας επηρεάσει μια εκτός ρεύματος. Ελέγξτε για να δείτε εάν υπάρχει μια τρέχουσα κατάσταση: [Κατάσταση υγείας Azure.](https://status.azure.com/status/history/)

Αποσυνδεθείτε από όλες τις ενεργές περιόδους λειτουργίας Azure. Ξεκινήστε μια λειτουργία in-private ή incognito του προγράμματος περιήγησης Web.

Μπορείτε επίσης να δοκιμάσετε να ανανεώσετε το πρόγραμμα περιήγησης, να χρησιμοποιήσετε ένα άλλο πρόγραμμα περιήγησης, να διαγράψετε τα cookies cache, εάν δεν λειτουργούν τα παραπάνω.

Μάθετε περισσότερα: [Αντιμετώπιση προβλημάτων σύνδεσης](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**Δεν είναι δυνατή η πρόσβαση σε συνδρομές**

Στην πύλη [Azure,](https://portal.azure.com/)βεβαιωθείτε ότι ο σωστός κατάλογος Azure είναι επιλεγμένος από το λογαριασμό στην επάνω δεξιά πλευρά.

Στο κέντρο [λογαριασμών Azure,](https://account.windowsazure.com/Subscriptions)βεβαιωθείτε ότι ο λογαριασμός που χρησιμοποιείται είναι ο διαχειριστής του λογαριασμού.

Μάθετε περισσότερα: Αντιμετώπιση [προβλημάτων που δεν βρέθηκαν συνδρομές](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**Δεν είναι δυνατή η πρόσβαση στο ιστορικό χρεώσεων**

Ο διαχειριστής λογαριασμού πρέπει να βεβαιωθεί ότι ο χρήστης που έχει πρόσβαση στις πληροφορίες χρέωσης προστίθεται στην υπηρεσία καταλόγου Azure Active directory ως χρήστης-επισκέπτης: [Προσθήκη ή διαγραφή νέου χρήστη.](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support)

Στη συνέχεια, ο χρήστης πρέπει να έχει έναν ρόλο καθολικού διαχειριστή: [Αναθέστε ρόλο στους χρήστες.](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support)

Δημοσιεύστε αυτό το μήνυμα, μπορείτε να αποκτήσετε πρόσβαση χρέωσης στο χρήστη χρησιμοποιώντας τις πολιτικές RBAC: [Εκχώρηση πρόσβασης στη χρέωση.](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)

**Προτεινόμενα έγγραφα**

-   [Δεν μπορώ να πραγματοποιήσω είσοδο για να διαχειριστώ τη συνδρομή μου στο Azure](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)