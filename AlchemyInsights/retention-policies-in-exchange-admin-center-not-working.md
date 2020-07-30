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
ms.openlocfilehash: 4d3ca121c8d22a0900f136f7f2a754dfb5b435f5
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522807"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Πολιτικές διατήρησης στο Κέντρο διαχείρισης του Exchange

Αν θέλετε να εκτελέσουμε αυτοματοποιημένους ελέγχους για τις ρυθμίσεις που αναφέρονται παρακάτω, επιλέξτε το κουμπί "Πίσω" <-- στο επάνω μέρος αυτής της σελίδας και, στη συνέχεια, πληκτρολογήστε τη διεύθυνση ηλεκτρονικού ταχυδρομείου του χρήστη που έχει προβλήματα με τις πολιτικές διατήρησης.

 **Τεύχος:** Οι πολιτικές διατήρησης που δημιουργήθηκαν ή ενημερώθηκαν πρόσφατα στο Κέντρο διαχείρισης του Exchange δεν εφαρμόζονται σε γραμματοκιβώτια ή στοιχεία, οι οποίοι δεν μετακινούνται στο γραμματοκιβώτιο αρχειοθέτησης ή δεν διαγράφονται. 
  
 **Ριζικές αιτίες:**
  
- Αυτό μπορεί να συμβαίνει επειδή ο **Βοηθός διαχειριζόμενων φακέλων** δεν έχει επεξεργαστεί το γραμματοκιβώτιο του χρήστη. Ο Βοηθός διαχειριζόμενων φακέλων προσπαθεί να επεξεργάζεται κάθε γραμματοκιβώτιο στον οργανισμό σας που βασίζεται στο cloud μία φορά κάθε επτά ημέρες. Εάν αλλάξετε μια ετικέτα διατήρησης ή εφαρμόσετε μια διαφορετική πολιτική διατήρησης σε ένα γραμματοκιβώτιο, μπορείτε να περιμένετε μέχρι το Πρόγραμμα βοήθειας διαχειριζόμενου φακέλου να επεξεργαστεί το γραμματοκιβώτιο ή μπορείτε να εκτελέσετε το cmdlet Start-ManagedFolderAssistant για να ξεκινήσετε το Βοηθό διαχειριζόμενων φακέλων για να επεξεργαστείτε ένα συγκεκριμένο γραμματοκιβώτιο. Η εκτέλεση αυτού του cmdlet είναι χρήσιμη για τον έλεγχο ή την αντιμετώπιση προβλημάτων μιας πολιτικής διατήρησης ή των ρυθμίσεων ετικέτας διατήρησης. Για περισσότερες πληροφορίες, επισκεφθείτε την επιλογή [Εκτέλεση του Βοηθού διαχειριζόμενων φακέλων](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Λύση:** Εκτελέστε την ακόλουθη εντολή για να ξεκινήσετε το Βοηθό διαχειριζόμενων φακέλων για ένα συγκεκριμένο γραμματοκιβώτιο:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Αυτό μπορεί επίσης να συμβεί εάν **το Retendhold** έχει **ενεργοποιηθεί** στο γραμματοκιβώτιο. Εάν το γραμματοκιβώτιο έχει τοποθετηθεί σε ένα Retenten that The reten that, η πολιτική διατήρησης στο γραμματοκιβώτιο δεν θα υποβληθεί σε επεξεργασία κατά τη διάρκεια αυτής της περιόδου. Για περισσότερες πληροφορίες σχετικά με τη ρύθμιση Retenten παρακρατήστε: [Διατήρηση γραμματοκιβωτίου .](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)
    
    **Λύση:**
    
  - Ελέγξτε την κατάσταση της ρύθμισης Retenten the retendoiseHold στο συγκεκριμένο γραμματοκιβώτιο στο [powershell EXO](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Εκτελέστε την ακόλουθη εντολή για να **απενεργοποιήσετε** το Retententen εκ των τες δύο σε ένα συγκεκριμένο γραμματοκιβώτιο:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Τώρα, εκτελέστε εκ νέου το Βοηθό διαχειριζόμενων φακέλων:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Σημείωση:** Εάν ένα γραμματοκιβώτιο είναι μικρότερο από 10 MB, ο Βοηθός διαχειριζόμενων φακέλων δεν θα επεξεργαστεί αυτόματα το γραμματοκιβώτιο.
 
Για περισσότερες πληροφορίες σχετικά με τις πολιτικές διατήρησης στο Κέντρο διαχείρισης του Exchange, ανατρέξτε στα θέματα:
- [Ετικέτες διατήρησης και πολιτικές διατήρησης](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Εφαρμογή πολιτικής διατήρησης σε γραμματοκιβώτια](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Προσθήκη ή κατάργηση ετικετών διατήρησης](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Τρόπος αναγνώρισης του τύπου διατήρησης που τοποθετείται σε ένα γραμματοκιβώτιο](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
