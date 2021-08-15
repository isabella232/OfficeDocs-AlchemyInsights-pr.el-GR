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
ms.openlocfilehash: 7377f77b7295e8134673c9a46fa7606842d4df949f535878d13986c6d39d0b5e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53993893"
---
# <a name="delete-tenant"></a>Διαγραφή μισθωτή

Για να διαγράψετε ένα Azure AD, βεβαιωθείτε ότι:
- Είστε καθολικός διαχειριστής στον κατάλογο.
- ΔΕΝ έχετε εισέλθει με ένα λογαριασμό που έχει τον προεπιλεγμένο κατάλογο, όπως contoso.onmicrosoft.com στον λογαριασμό που είναι συνδεδεμένος-- όπως admin@contoso.onmicrosoft.com.
- Καταργήστε τυχόν ενεργές εφαρμογές στον κατάλογο πριν από τη διαγραφή. Για να καταργήσετε ενεργές εφαρμογές, μεταβείτε στις καταχωρήσεις εφαρμογών και καταργήστε τις υπάρχουσες εφαρμογές.
- Δεν υπάρχουν ενεργές συνδρομές για οποιεσδήποτε υπηρεσίες Microsoft Online Services, όπως Microsoft Azure, Office 365 ή Azure AD Premium που σχετίζονται με τον κατάλογο. Μεταφέρετε τις συνδρομές σας ή επισπεύψτε την ακύρωση ενεργών συνδρομών μέσω της Υποστήριξης και χρέωσης του Azure. Μάθετε περισσότερα σχετικά με τον τρόπο ακύρωσης Office 365 και τις συνδρομές Azure. Για οδηγίες σχετικά με τη συσχέτιση ή την προσθήκη μιας υπάρχουσας συνδρομής σε ένα μισθωτή, ανατρέξτε στο θέμα Συσχέτιση ή προσθήκη [συνδρομής Azure στο μισθωτή Azure AD.](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory)
- Δεν υπάρχει ενεργή άδεια χρήσης. Για να καταργήσετε άδειες χρήσης, ανατρέξτε [στο θέμα Τρόπος κατάργησης της συνδρομής για την κατάργηση άδειας χρήσης.](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription)
- Δεν υπάρχουν άλλοι ενεργοί χρήστες στον κατάλογο εκτός από εσάς ως καθολικός διαχειριστής όταν προσπαθείτε να διαγράψετε το Azure AD. Καταργήστε τυχόν άλλους ενεργούς χρήστες και τυχόν εξαρτήσεις από ένα προσαρμοσμένο όνομα τομέα στο μισθωτή θα πρέπει επίσης να καταργηθούν, όπως οι χρήστες που έχουν δημιουργηθεί με admin@contoso.com.

Για περισσότερες λεπτομέρειες σχετικά με τον τρόπο με τον οποίο μπορείτε να κάνετε τα εξής:
- Διαγράψτε "Azure Active Directory" ή "συνδρομή", ανατρέξτε στο [θέμα Διαγραφή Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto)
- Κατάργηση εφαρμογών στον κατάλογο, ανατρέξτε στο θέμα [Κατάργηση εφαρμογών.](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app) 
