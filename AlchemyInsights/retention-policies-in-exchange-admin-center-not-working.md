---
title: Οι πολιτικές διατήρησης στο Κέντρο διαχείρισης του Exchange δεν λειτουργεί
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 5d7b62546397c13b37540e8797b31123b2880280
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551343"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Οι πολιτικές διατήρησης στο Κέντρο διαχείρισης του Exchange

 **Θέμα:** Που δημιουργήθηκαν πρόσφατα ή πολιτικές διατήρησης ενημερωμένο στο Κέντρο διαχείρισης Exchange δεν εφαρμόζουν γραμματοκιβώτια ή στοιχεία δεν μετακινούνται στο γραμματοκιβώτιο αρχειοθέτηση ή διαγραφή. 
  
 **Βασικές αιτίες:**
  
- Αυτό μπορεί να οφείλεται η **Διαχείριση Βοηθός φακέλου** δεν επεξεργάστηκε το γραμματοκιβώτιο του χρήστη. Η διαχείριση Βοηθός φακέλου προσπαθεί να επεξεργαστεί κάθε γραμματοκιβώτιο στον οργανισμό σας βασίζεται στο νέφος μία φορά κάθε επτά ημέρες. Εάν αλλάξετε μια ετικέτα διατήρησης ή εφαρμόζεται διαφορετική πολιτική διατήρησης σε ένα γραμματοκιβώτιο, μπορείτε να περιμένετε μέχρι η διαχειριζόμενη φάκελο επικουρεί επεξεργάζεται το γραμματοκιβώτιο, ή μπορείτε να εκτελέσετε το cmdlet έναρξης-ManagedFolderAssistant για να ξεκινήσετε τη Διαχείριση Βοηθός φακέλου για να επεξεργαστείτε μια συγκεκριμένη γραμματοκιβώτιο. Εκτέλεση αυτού του cmdlet είναι χρήσιμη για τη δοκιμή ή την αντιμετώπιση προβλημάτων μια πολιτική διατήρησης ή ρυθμίσεις ετικέτα διατήρησης. Για περισσότερες πληροφορίες, επισκεφθείτε την [Εκτέλεση διαχειριζόμενου Βοηθός φακέλου](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Λύση:** Εκτελέστε την ακόλουθη εντολή για να ξεκινήσετε τη Διαχείριση Βοηθός φακέλου για ένα συγκεκριμένο γραμματοκιβώτιο:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Αυτό μπορεί να συμβεί επίσης αν **RetentionHold** έχει **ενεργοποιηθεί** στο γραμματοκιβώτιο. Εάν το γραμματοκιβώτιο έχει τοποθετηθεί σε ένα RetentionHold, δεν θα γίνει επεξεργασία της πολιτικής διατήρησης στο γραμματοκιβώτιο σε αυτό το διάστημα. Για περισσότερες informaton, δείτε: ρύθμιση της RetentionHold: [Κρατήστε διατήρησης γραμματοκιβωτίου](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Λύση:**
    
  - Ελέγξτε την κατάσταση της ρύθμισης RetentionHold στο συγκεκριμένο γραμματοκιβώτιο σε [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Εκτελέστε την ακόλουθη εντολή για να **απενεργοποιήσετε** RetentionHold για ένα συγκεκριμένο γραμματοκιβώτιο:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Τώρα, εκτελέστε ξανά το φάκελο διαχειριζόμενες Βοηθός:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Σημείωση:** Εάν ένα γραμματοκιβώτιο είναι μικρότερο από 10 MB, η διαχείριση Βοηθός φακέλου θα γίνει αυτόματα επεξεργασία στο γραμματοκιβώτιο.
 
Για περισσότερες πληροφορίες σχετικά με τις πολιτικές διατήρησης στο Κέντρο διαχείρισης Exchange, ανατρέξτε στο θέμα:
- [Ετικέτες διατήρησης και πολιτικές διατήρησης](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Εφαρμογή πολιτικής διατήρησης σε γραμματοκιβώτια](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Προσθήκη ή κατάργηση ετικετών διατήρησης](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Τον τρόπο αναγνώρισης του τύπου των παραδιδόμενων τοποθετείται σε ένα γραμματοκιβώτιο](https://docs.microsoft.com/office365/securitycompliance/identify-a-hold-on-an-exchange-online-mailbox)
