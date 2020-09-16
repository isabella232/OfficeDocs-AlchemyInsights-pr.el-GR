---
title: Θέματα άδειας χρήσης του Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: f0a7625c7b77860e5ba0e29f2df47101749aace3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47657276"
---
# <a name="yammer-licensing-issues"></a>Θέματα άδειας χρήσης του Yammer

Όλοι οι χρήστες πρέπει να διαθέτουν άδεια χρήσης της υπηρεσίας Enterprise του Yammer, αλλά από προεπιλογή το Yammer δεν απαιτεί από τους χρήστες να διαθέτουν άδεια χρήσης για πρόσβαση στην υπηρεσία. Όταν ένας διαχειριστής αλλάξει τη ρύθμιση για να αποκλείσει τους χρήστες του Microsoft 365 χωρίς άδειες χρήσης του Yammer, οι χρήστες που δεν έχουν αντιστοιχιστεί σε μια άδεια χρήσης Yammer Enterprise δεν έχουν πρόσβαση στην υπηρεσία Yammer. Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα Διαχείριση αδειών χρήσης του Yammer στο Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

Όταν οι άδειες χρήσης καταργούνται από τους χρήστες, το πλακίδιο Yammer δεν εμφανίζεται πλέον και άλλες υπηρεσίες μπορούν να χρησιμοποιήσουν την κατάργηση αδειών χρήσης για να αποκρύψουν δυνατότητες. Σε άλλες περιπτώσεις, οι δυνατότητες μπορεί να εξακολουθούν να εμφανίζονται, αλλά απαιτούν εκχώρηση άδειας χρήσης για λειτουργία.  

**Δεν γίνεται ενημέρωση της άδειας χρήσης για το χρήστη**  

Περιστασιακά, ένας χρήστης έχει εκχωρηθεί μια άδεια χρήσης, αλλά εξακολουθεί να μην είναι δυνατό να αποκτήσει πρόσβαση στο Yammer. Οι καθυστερήσεις είναι πιθανότερο να προκύψουν όταν μια ανάθεση μαζικών αδειών χρήσης βρίσκεται σε εξέλιξη. Οι χρήστες του Yammer μπορεί να μην ενημερώνονται με την ίδια σειρά που αλλάζουν οι άδειες χρήσης στο Azure AD, επειδή το σύστημα εκτελείται ασύγχρονα. Περιμένετε έως και 24 ώρες πριν από το άνοιγμα μιας υπόθεσης υποστήριξης για την αναφορά ζητημάτων συγχρονισμού άδειας χρήσης.  

**Εκχώρηση μαζικών αδειών χρήσης**  

Οι άδειες χρήσης μπορούν να εκχωρηθούν μέσω του κέντρου διαχείρισης ή των δεσμών ενεργειών του PowerShell. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [εκχώρηση αδειών χρήσης σε χρήστες](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) και [εκχώρηση αδειών χρήσης σε λογαριασμούς χρηστών με το Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell). 

Η υποστήριξη της Microsoft δεν παρέχει βοήθεια για τη δημιουργία δεσμών ενεργειών, αλλά είναι διαθέσιμη η τεκμηρίωση για την εκχώρηση αδειών χρήσης του Yammer. Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα Διαχείριση αδειών χρήσης του Yammer με χρήση του Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).