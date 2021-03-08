---
title: Αρχεία καταγραφής κωδικών πρόσβασης
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9361"
- "9003259"
ms.openlocfilehash: ed151b436fa2043c610931deeb74a202af88fcf4
ms.sourcegitcommit: 226fe97678b6be215eda0c278399f8be9be525c1
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50525138"
---
# <a name="password-logs"></a>Αρχεία καταγραφής κωδικών πρόσβασης

**Έχω προβλήματα κατά την πρόσβαση σε αρχεία καταγραφής ελέγχου επαναφοράς κωδικού πρόσβασης**

Για την αντιμετώπιση προβλημάτων σχετικά με την πρόσβαση σε αρχεία καταγραφής ελέγχου επαναφοράς κωδικού πρόσβασης, εκτελέστε το παρακάτω βήμα:

Βεβαιωθείτε ότι είστε εξουσιοδοτημένοι για την προβολή των αρχείων καταγραφής ελέγχου. 

Μόνο οι παρακάτω ρόλοι είναι εξουσιοδοτημένοι:
 - Καθολικός διαχειριστής
 - Διαχειριστής ασφαλείας
 - Πρόγραμμα ανάγνωσης ασφαλείας

**Θέλω να δω όλα τα συμβάντα ελέγχου επαναφοράς κωδικού πρόσβασης από τη στιγμή που αναπτύξαμε αρχικά**

Έως και 120.000 συμβάντα επαναφοράς/καταχώρησης κωδικού πρόσβασης αποθηκεύονται στις αναφορές των τελευταίων 30 ημερών. Αυτό το μέγιστο όριο ισχύει για το περιβάλλον εργασίας χρήστη κατά τη λήψη του CSV. 1 εκατομμύριο συμβάντα είναι διαθέσιμες μέσω του PowerShell.
Για περισσότερες πληροφορίες, ανατρέξτε στις παρακάτω συνδέσεις:

- [Συμβάντα επαναφοράς κωδικού πρόσβασης από το χρήστη από το API αναφορών και συμβάντων του Azure AD](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Πώς μπορείτε να κάνετε λήψη συμβάντων καταχώρησης επαναφοράς κωδικού πρόσβασης γρήγορα με το PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

**Θέλω να κατανοήσω περισσότερα σχετικά με τις δυνατότητες αναφοράς επαναφοράς κωδικού πρόσβασης**

Ελέγξτε ποιος καταχωρεί ή επαναφέρει κωδικούς πρόσβασης με αρχεία καταγραφής ελέγχου επαναφοράς κωδικού πρόσβασης του Azure AD στην πύλη Azure, στην περιοχή Χρήστες **και ομάδες.**
Για περισσότερες πληροφορίες, ανατρέξτε στις παρακάτω συνδέσεις:

- [Επισκόπηση αναφορών επαναφοράς κωδικού πρόσβασης](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Πώς μπορείτε να προβάλετε αναφορές επαναφοράς κωδικού πρόσβασης στην πύλη Azure](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Συμβάντα επαναφοράς κωδικού πρόσβασης από το χρήστη από το API αναφορών και συμβάντων του Azure AD](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Πώς μπορείτε να κάνετε λήψη συμβάντων καταχώρησης επαναφοράς κωδικού πρόσβασης γρήγορα με το PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


