---
title: Οι πολιτικές διατήρησης στο κέντρο διαχείρισης του Exchange δεν λειτουργούν
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 1fee2361b2dd6e0989d430a17aebb13bd5948578
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740510"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Πολιτικές διατήρησης στο κέντρο διαχείρισης του Exchange

Εάν θέλετε να εκτελέσουμε αυτοματοποιημένους ελέγχους για τις ρυθμίσεις που αναφέρονται παρακάτω, επιλέξτε το κουμπί πίσω <--στο επάνω μέρος αυτής της σελίδας και, στη συνέχεια, πληκτρολογήστε τη διεύθυνση ηλεκτρονικού ταχυδρομείου του χρήστη που έχει προβλήματα με τις πολιτικές διατήρησης.

 **Πρόβλημα:** Οι πρόσφατα δημιουργημένες ή ενημερωμένες πολιτικές διατήρησης στο κέντρο διαχείρισης του Exchange δεν εφαρμόζονται σε γραμματοκιβώτια ή τα στοιχεία δεν μετακινούνται στο γραμματοκιβώτιο αρχειοθέτησης ή διαγράφονται. 
  
 **Ριζικές αιτίες:**
  
- Αυτό μπορεί να συμβαίνει επειδή ο **Βοηθός διαχειριζόμενου φακέλου** δεν έχει επεξεργαστεί το γραμματοκιβώτιο του χρήστη. Ο βοηθός διαχειριζόμενου φακέλου επιχειρεί να επεξεργαστεί κάθε γραμματοκιβώτιο στον οργανισμό σας που βασίζεται στο cloud μία φορά κάθε επτά ημέρες. Εάν αλλάξετε μια ετικέτα διατήρησης ή εφαρμόζετε μια διαφορετική πολιτική διατήρησης σε ένα γραμματοκιβώτιο, μπορείτε να περιμένετε μέχρι ο διαχειριζόμενος φάκελος να βοηθήσει την επεξεργασία του γραμματοκιβωτίου ή μπορείτε να εκτελέσετε το cmdlet εκκίνησης-ManagedFolderAssistant για να ξεκινήσετε τον βοηθό διαχειριζόμενου φακέλου για να επεξεργαστείτε ένα συγκεκριμένο γραμματοκιβώτιο. Η εκτέλεση αυτού του cmdlet είναι χρήσιμη για τον έλεγχο ή την αντιμετώπιση προβλημάτων μιας πολιτικής διατήρησης ή ρυθμίσεων ετικετών διατήρησης. Για περισσότερες πληροφορίες, επισκεφθείτε [την εκτέλεση του βοηθού διαχειριζόμενου φακέλου](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Λύση:** Εκτελέστε την ακόλουθη εντολή για να ξεκινήσετε το βοηθό διαχειριζόμενου φακέλου για ένα συγκεκριμένο γραμματοκιβώτιο:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Αυτό μπορεί επίσης να προκύψει εάν το **RetentionHold** έχει **ενεργοποιηθεί** στο γραμματοκιβώτιο. Εάν το γραμματοκιβώτιο έχει τοποθετηθεί σε ένα RetentionHold, η πολιτική διατήρησης στο γραμματοκιβώτιο δεν θα υποβληθεί σε επεξεργασία στη διάρκεια αυτού του χρόνου. Για περισσότερες informaton στη ρύθμιση RetentionHold, ανατρέξτε στο θέμα: [διατήρηση διατήρησης γραμματοκιβωτίου](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Λύση**
    
  - Επιλέξτε την κατάσταση της ρύθμισης RetentionHold στο συγκεκριμένο γραμματοκιβώτιο στο [έξω PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Εκτελέστε την ακόλουθη εντολή για να **απενεργοποιήσετε** το RetentionHold σε ένα συγκεκριμένο γραμματοκιβώτιο:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Τώρα, εκτελέστε ξανά το βοηθό διαχειριζόμενου φακέλου:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Σημείωση:** Εάν ένα γραμματοκιβώτιο είναι μικρότερο από 10 MB, ο διαχειριζόμενος Βοηθός φακέλου δεν θα επεξεργαστεί αυτόματα το γραμματοκιβώτιο.
 
Για περισσότερες πληροφορίες σχετικά με τις πολιτικές διατήρησης στο κέντρο διαχείρισης του Exchange, ανατρέξτε στα θέματα:
- [Ετικέτες διατήρησης και πολιτικές διατήρησης](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Εφαρμογή πολιτικής διατήρησης σε γραμματοκιβώτια](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Προσθήκη ή κατάργηση ετικετών διατήρησης](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Πώς μπορείτε να προσδιορίσετε τον τύπο της διατήρησης που τοποθετείται σε ένα γραμματοκιβώτιο](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
