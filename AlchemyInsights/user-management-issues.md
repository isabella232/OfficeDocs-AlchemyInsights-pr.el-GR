---
title: Ζητήματα διαχείρισης χρηστών
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9209"
- "9005371"
ms.openlocfilehash: 4b61686381de0cafa38857ca7a96b3a81aa191ec
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036281"
---
# <a name="user-management-issues"></a>Ζητήματα διαχείρισης χρηστών

**Τι συμβαίνει με τους τρέχοντες χρήστες που έχουν εκχωρηθεί στην εφαρμογή εάν απενεργοποιήσω την ιδιότητα "Απαιτείται ανάθεση χρήστη" (ορίστε αυτή την ιδιότητα σε "Όχι";**

Η απενεργοποίηση της **απαιτούμενης ανάθεσης εργασίας** χρήστη ΔΕΝ επηρεάζει τους χρήστες που έχουν αντιστοιχιστεί τη συγκεκριμένη στιγμή. Η απενεργοποίηση αυτής της ιδιότητας θα επιτρέψει μόνο σε όλους τους χρήστες να αποκτήσουν πρόσβαση στην εφαρμογή. Όλοι οι χρήστες που παρατίθενται και οι χρήστες που έχουν αντιστοιχιστεί σε ομάδες στην εφαρμογή θα εξακολουθούν να είναι έγκυροι.

- Για να περιορίσετε την εφαρμογή σας σε συγκεκριμένο σύνολο χρηστών, ανατρέξτε στο θέμα - Περιορισμός εφαρμογής Azure AD σε ένα σύνολο χρηστών [- Πλατφόρμα ταυτότητας της Microsoft | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.).
- Για να εκχωρήσετε χρήστες και ομάδες, σε εταιρικές εφαρμογές στο Azure Active Directory (Azure AD), είτε μέσα από την πύλη Azure είτε χρησιμοποιώντας το PowerShell, ανατρέξτε στο θέμα Διαχείριση ανάθεσης χρηστών για μια εφαρμογή [στο Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal)
- Για να αναθέσετε δικαιώματα δημιουργίας και διαχείρισης εφαρμογών, ανατρέξτε στο θέμα Δικαιώματα διαχειριστή εφαρμογών [πληρεξουσίου - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles).
- **Απόκρυψη συγκεκριμένων εταιρικών εφαρμογών από χρήστες** - Ακολουθήστε τα παρακάτω βήματα για να αποκρύψετε όλες τις εφαρμογές του Microsoft 365 από τον **πίνακα MyApps.** Οι εφαρμογές θα εξακολουθούν να είναι ορατές στην πύλη του Office 365.

 1. Πραγματοποιήστε είσοδο στην πύλη Azure ως καθολικός διαχειριστής για τον κατάλογο. 
 2. Επιλέξτε **Azure Active Directory.** 
 3. Επιλέξτε **"Χρήστες".** 
 4. Επιλέξτε **"Ρυθμίσεις χρήστη".** 
 5. Στην περιοχή **"Εταιρικές εφαρμογές",** κάντε **κλικ στην επιλογή "Διαχείριση του πώς οι τελικοί χρήστες εκκινούν και προβάλλουν τις εφαρμογές τους".** 
 6. Για **τους χρήστες μπορούν να δουν μόνο τις εφαρμογές του Office 365 στην πύλη του Office 365, κάντε κλικ** στο κουμπί **"Ναι".** 
 7. Επιλέξτε **Αποθήκευση**. 
 8. Για περισσότερες λεπτομέρειες, [ανατρέξτε στο θέμα Απόκρυψη εταιρικής εφαρμογής από την εμπειρία χρήστη στο Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)

- Εάν προσφέρετε μια εφαρμογή Λογισμικού ως υπηρεσία (SaaS) σε πολλούς οργανισμούς, μπορείτε να ρυθμίσετε τις παραμέτρους της εφαρμογής σας ώστε να αποδέχεται τις είσοδοι από οποιονδήποτε μισθωτή azure Active Directory (Azure AD). Αυτή η ρύθμιση παραμέτρων ονομάζεται "δημιουργία πολλών μισθωτών της εφαρμογής σας". Οι χρήστες σε οποιονδήποτε μισθωτή του Azure AD θα μπορούν να πραγματοποιήσουν είσοδο στην εφαρμογή σας αφού συναινέσει στη χρήση του λογαριασμού τους με την εφαρμογή σας. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα Δημιουργία εφαρμογών που θα πραγματοποιήσουν είσοδο σε χρήστες [του Azure AD - Πλατφόρμα ταυτότητας της Microsoft | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant).

- **Πώς μπορεί ένας τελικός χρήστης να αποκτήσει πρόσβαση στην εφαρμογή μετά την εκχωρήσεή του στην εφαρμογή;**

Κάθε εφαρμογή στο Enterprise Application Blade διαθέτει μια σύνδεση για πρόσβαση στους τελικούς χρήστες. Οι χρήστες μπορούν επίσης να αποκτήσουν πρόσβαση στην **εφαρμογή μέσω της πύλης Myapps** με εύκολο τρόπο.

- **Θέλετε να μάθετε ποιες εφαρμογές και τον τύπο εφαρμογών χρησιμοποιούνται από τους χρήστες;**

Μπορείτε να κάνετε λήψη αναφορών σύνδεσης για τις τελευταίες 30 ημέρες **από portal.azure.com > Azure Active directory> signins> να κάνετε λήψη αναφορών.**

- Μάθετε πώς μπορείτε να [εκχωρήσετε σε ένα μισθωτή ευρεία συγκατάθεση διαχειριστή σε μια εφαρμογή και να ρυθμίσετε](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) τον [τρόπο με τον οποίο οι τελικοί χρήστες συναινούν σε εφαρμογές.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent)

- Κατανοήστε [πώς λειτουργεί η συγκατάθεση](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) και [διαχειριστείτε τη συγκατάθεση για τις εφαρμογές.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests)


