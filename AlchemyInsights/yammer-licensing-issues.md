---
title: Ζητήματα αδειών χρήσης του Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 6d9b2126dc1ed90968738ddb2e249dce9857f1db
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148239"
---
# <a name="yammer-licensing-issues"></a>Ζητήματα αδειών χρήσης του Yammer

Όλοι οι χρήστες πρέπει να έχουν άδεια χρήσης της υπηρεσίας Yammer Enterprise, αλλά από προεπιλογή το Yammer δεν απαιτεί οι χρήστες να έχουν άδεια πρόσβασης στην υπηρεσία. Όταν ένας διαχειριστής αλλάζει τη ρύθμιση για να αποκλείσει χρήστες του Microsoft 365 χωρίς άδειες χρήσης yammer, οι χρήστες στους οποίο δεν έχει εκχωρηθεί άδεια χρήσης yammer enterprise δεν μπορούν να αποκτήσουν πρόσβαση στην υπηρεσία Yammer. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Διαχείριση αδειών χρήσης του Yammer στο Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

Όταν καταργούνται άδειες χρήσης από τους χρήστες, το πλακίδιο Yammer δεν εμφανίζεται πλέον και άλλες υπηρεσίες μπορούν να χρησιμοποιήσουν την κατάργηση άδειας χρήσης για την απόκρυψη δυνατοτήτων. Σε άλλες περιπτώσεις, οι δυνατότητες μπορούν ακόμα να εμφανίζονται, αλλά απαιτούν εκχώρηση άδειας για να λειτουργήσουν.  

**Η άδεια χρήσης δεν ενημερώνεται για το χρήστη**  

Περιστασιακά, ένας χρήστης εκχωρείται μια άδεια χρήσης, αλλά εξακολουθεί να μην είναι σε θέση να αποκτήσει πρόσβαση στο Yammer. Οι καθυστερήσεις είναι πιο πιθανό να προκύψουν όταν μια μαζική εκχώρηση άδειας χρήσης βρίσκεται σε εξέλιξη. Οι χρήστες του Yammer ενδέχεται να μην ενημερώνονται με την ίδια σειρά με τις άδειες χρήσης που αλλάζουν στο Azure AD, επειδή το σύστημα εκτελείται ασύγχρονα. Περιμένετε έως και 24 ώρες πριν ανοίξετε μια υπόθεση υποστήριξης για να αναφέρετε προβλήματα συγχρονισμού άδειας χρήσης.  

**Μαζική εκχώρηση άδειας χρήσης**  

Οι άδειες χρήσης μπορούν να εκχωρηθούν μέσω του κέντρου διαχείρισης ή των δεσμών ενεργειών powershell. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Εκχώρηση αδειών χρήσης σε χρήστες](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) και [Εκχώρηση αδειών χρήσης σε λογαριασμούς χρηστών με το Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell). 

Η Υποστήριξη της Microsoft δεν παρέχει βοήθεια για τη δημιουργία δεσμών ενεργειών, αλλά είναι διαθέσιμη τεκμηρίωση σχετικά με την εκχώρηση άδειας χρήσης yammer. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Διαχείριση αδειών χρήσης yammer χρησιμοποιώντας το Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).