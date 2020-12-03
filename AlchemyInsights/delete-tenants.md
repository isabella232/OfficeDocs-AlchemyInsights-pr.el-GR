---
title: Διαγραφή μισθωτή
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564621"
---
# <a name="delete-tenant"></a>Διαγραφή μισθωτή

Για να διαγράψετε μια AD Azure, βεβαιωθείτε ότι:
- Είστε καθολικός διαχειριστής στον κατάλογο.
- Δεν έχετε εισέλθει με ένα λογαριασμό που έχει τον προεπιλεγμένο κατάλογο, όπως το contoso.onmicrosoft.com στο λογαριασμό που έχει υπογραφεί, όπως το admin@contoso.onmicrosoft.com.
- Καταργήστε τυχόν ενεργές εφαρμογές στον κατάλογο πριν από τη διαγραφή. Για να καταργήσετε τις ενεργές εφαρμογές, μεταβείτε στις καταχωρήσεις εφαρμογών και καταργήστε τις υπάρχουσες εφαρμογές.
- Δεν υπάρχουν ενεργές συνδρομές για οποιαδήποτε Microsoft Online Services, όπως το Microsoft Azure, το Office 365 ή το Azure AD Premium που σχετίζεται με τον κατάλογο. Μεταφέρετε τις συνδρομές σας ή επιταχύνετε την ακύρωση των ενεργών συνδρομών μέσω υποστήριξης Azure και χρέωσης. Μάθετε περισσότερα σχετικά με το πώς μπορείτε να ακυρώσετε τις συνδρομές του Office 365 και του Azure. Για οδηγίες σχετικά με τη συσχέτιση ή την προσθήκη μιας υπάρχουσας συνδρομής σε έναν μισθωτή, ανατρέξτε στο θέμα [συσχέτιση ή προσθήκη μιας συνδρομής Azure στον ΜΙΣΘΩΤΉ AD Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).
- Δεν υπάρχει ενεργή άδεια χρήσης. Για να καταργήσετε άδειες χρήσης, ανατρέξτε στο θέμα [Πώς να καταργήσετε τη συνδρομή για να καταργήσετε την άδεια χρήσης](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).
- Δεν υπάρχουν άλλοι ενεργοί χρήστες στον κατάλογο εκτός από εσάς ως καθολικός διαχειριστής, όταν προσπαθείτε να διαγράψετε το Azure AD. Καταργήστε τυχόν άλλους ενεργούς χρήστες και οποιεσδήποτε εξαρτήσεις σε ένα προσαρμοσμένο όνομα τομέα στον μισθωτή θα πρέπει επίσης να καταργηθούν, όπως οι χρήστες που έχουν δημιουργηθεί με το admin@contoso.com.

Για περισσότερες λεπτομέρειες, μπορείτε να κάνετε τα εξής:
- Διαγράψτε τη φράση "Azure Active Directory" ή "συνδρομή", ανατρέξτε στο θέμα [Διαγραφή υπηρεσίας καταλόγου Active Directory Azure](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).
- Κατάργηση εφαρμογών στον κατάλογο, ανατρέξτε στο θέμα [Κατάργηση εφαρμογών](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app). 
