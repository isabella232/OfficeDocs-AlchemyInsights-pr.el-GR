---
title: Yammer παραχώρησης αδειών χρήσης
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
ms.openlocfilehash: 3ec764ece9cb7be933e9e2cd002379898522790528b0fa586ab501424b00cd7b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53989729"
---
# <a name="yammer-licensing-issues"></a>Yammer παραχώρησης αδειών χρήσης

Όλοι οι χρήστες πρέπει να έχουν άδεια χρήσης για να χρησιμοποιήσουν την Yammer Enterprise, αλλά από προεπιλογή Yammer δεν απαιτεί από τους χρήστες να έχουν άδεια χρήσης για να αποκτήσουν πρόσβαση στην υπηρεσία. Όταν ένας διαχειριστής αλλάξει τη ρύθμιση για να αποκλείσει Microsoft 365 χρήστες χωρίς άδειες χρήσης του Yammer, οι χρήστες που δεν έχουν εκχωρήσει μια άδεια χρήσης του Yammer Enterprise δεν μπορούν να αποκτήσουν πρόσβαση στην Yammer υπηρεσίας. Για περισσότερες πληροφορίες, [ανατρέξτε στο θέμα Yammer αδειών χρήσης στο Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

Όταν οι άδειες χρήσης καταργούνται από τους χρήστες, το πλακίδιο Yammer δεν εμφανίζεται πλέον και άλλες υπηρεσίες μπορούν να χρησιμοποιήσουν την κατάργηση άδειας χρήσης για να αποκρύψουν δυνατότητες. Σε άλλες περιπτώσεις, οι δυνατότητες εξακολουθούν να εμφανίζονται, αλλά απαιτούν τη λειτουργία εκχώρησης άδειας χρήσης.  

**Η άδεια χρήσης δεν ενημερώνεται για το χρήστη**  

Περιστασιακά, σε ένα χρήστη εκχωρείται μια άδεια χρήσης, αλλά εξακολουθεί να μην μπορεί να αποκτήσει πρόσβαση Yammer. Οι καθυστερήσεις είναι πιο πιθανό να προκύψουν όταν μια μαζική εκχώρηση άδειας χρήσης είναι σε εξέλιξη. Yammer οι χρήστες ενδέχεται να μην ενημερώνονται με την ίδια σειρά με τις άδειες χρήσης που αλλάζουν στο Azure AD, επειδή το σύστημα εκτελείται ασύγχρονα. Περιμένετε έως και 24 ώρες πριν ανοίξετε μια υπόθεση υποστήριξης για να αναφέρετε προβλήματα συγχρονισμού αδειών χρήσης.  

**Μαζική εκχώρηση άδειας χρήσης**  

Οι άδειες χρήσης μπορούν να εκχωρούνται μέσω του κέντρου διαχείρισης ή της δέσμης ενεργειών του PowerShell. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Εκχώρηση αδειών χρήσης σε χρήστες](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) και Εκχώρηση αδειών χρήσης σε [λογαριασμούς χρηστών με Office 365 PowerShell.](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell) 

Η Υποστήριξη της Microsoft δεν παρέχει βοήθεια σχετικά με τη δημιουργία δεσμών ενεργειών, αλλά υπάρχει τεκμηρίωση Yammer εκχώρησης άδειας χρήσης. Για περισσότερες πληροφορίες, [ανατρέξτε στο θέμα Yammer αδειών χρήσης χρησιμοποιώντας Windows PowerShell.](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell)