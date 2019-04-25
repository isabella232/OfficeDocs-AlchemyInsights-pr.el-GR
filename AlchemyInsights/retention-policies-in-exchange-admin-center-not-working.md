---
title: Οι πολιτικές διατήρησης στο Κέντρο διαχείρισης του Exchange δεν λειτουργεί
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: c9061fa728edaab6575a7b1027783e56739a6d14
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32371298"
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
  

