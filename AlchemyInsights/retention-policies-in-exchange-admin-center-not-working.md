---
title: Οι πολιτικές διατήρησης στο Κέντρο διαχείρισης του Exchange δεν λειτουργούν
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 3040365b9d686bcbcce60977ee9bdbbaffc70b24
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44502607"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Πολιτικές διατήρησης στο Κέντρο διαχείρισης του Exchange

 **Το θέμα:** Οι νέες πολιτικές διατήρησης που δημιουργήθηκαν πρόσφατα στο Κέντρο διαχείρισης του Exchange δεν εφαρμόζονται σε γραμματοκιβώτια ή τα στοιχεία δεν μετακινούνται στο γραμματοκιβώτιο αρχειοθέτησης ή διαγράφονται. 
  
 **Βασικές αιτίες:**
  
- Αυτό μπορεί να συμβαίνει επειδή ο **Βοηθός διαχειριζόμενου φακέλου** δεν έχει επεξεργαστεί το γραμματοκιβώτιο του χρήστη. Ο Βοηθός διαχειριζόμενου φακέλου προσπαθεί να επεξεργαστεί κάθε γραμματοκιβώτιο στον οργανισμό σας που βασίζεται στο cloud μία φορά κάθε επτά ημέρες. Εάν αλλάξετε μια ετικέτα διατήρησης ή εφαρμόσετε μια διαφορετική πολιτική διατήρησης σε ένα γραμματοκιβώτιο, μπορείτε να περιμένετε μέχρι το Πρόγραμμα υποβοήθησης διαχειριζόμενου φακέλου να επεξεργαστεί το γραμματοκιβώτιο ή μπορείτε να εκτελέσετε το cmdlet Start-ManagedFolderAssistant για να ξεκινήσετε το Βοηθό διαχειριζόμενου φακέλου για να επεξεργαστείτε ένα συγκεκριμένο γραμματοκιβώτιο. Η εκτέλεση αυτού του cmdlet είναι χρήσιμη για τον έλεγχο ή την αντιμετώπιση προβλημάτων μιας πολιτικής διατήρησης ή ρυθμίσεων ετικέτας διατήρησης. Για περισσότερες πληροφορίες, [επισκεφθείτε την επιλογή Εκτέλεση του Βοηθού διαχειριζόμενου φακέλου](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Η λύση:** Εκτελέστε την ακόλουθη εντολή για να ξεκινήσετε το Βοηθό διαχειριζόμενου φακέλου για ένα συγκεκριμένο γραμματοκιβώτιο:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Αυτό μπορεί επίσης να συμβεί εάν **το RetentionHold** έχει **ενεργοποιηθεί** στο γραμματοκιβώτιο. Εάν το γραμματοκιβώτιο έχει τοποθετηθεί σε ένα RetentionHold, η πολιτική διατήρησης στο γραμματοκιβώτιο δεν θα υποβληθεί σε επεξεργασία κατά τη διάρκεια αυτής της περιόδου. Για περισσότερες πληροφορίες σχετικά με τη ρύθμιση Διατήρηση διατήρησης, ανατρέξτε [στο θέμα: Διατήρηση γραμματοκιβωτίου Διατήρηση .](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)
    
    **Λύση:**
    
  - Ελέγξτε την κατάσταση της ρύθμισης Διατήρηση διατήρησης στο συγκεκριμένο γραμματοκιβώτιο στο [powershell EXO](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Εκτελέστε την ακόλουθη εντολή για να **απενεργοποιήσετε** το RetentionHold σε ένα συγκεκριμένο γραμματοκιβώτιο:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Τώρα, εκτελέστε εκ νέου το Βοηθό διαχειριζόμενου φακέλου:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Σημείωση:** Εάν ένα γραμματοκιβώτιο είναι μικρότερο από 10 MB, ο Βοηθός διαχειριζόμενου φακέλου δεν θα επεξεργαστεί αυτόματα το γραμματοκιβώτιο.
 
Για περισσότερες πληροφορίες σχετικά με τις πολιτικές διατήρησης στο Κέντρο διαχείρισης του Exchange, ανατρέξτε στα θέματα:
- [Ετικέτες διατήρησης και πολιτικές διατήρησης](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Εφαρμογή πολιτικής διατήρησης σε γραμματοκιβώτια](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Προσθήκη ή κατάργηση ετικετών διατήρησης](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Τρόπος αναγνώρισης του τύπου διατήρησης που τοποθετείται σε ένα γραμματοκιβώτιο](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
