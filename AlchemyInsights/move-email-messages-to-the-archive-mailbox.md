---
title: Μετακίνηση μηνυμάτων ηλεκτρονικού ταχυδρομείου στο γραμματοκιβώτιο αρχειοθέτησης
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: a631af20e28a531a40f078e290239a372c38ab74
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29941709"
---
Αντιμετωπίζετε προβλήματα Αρχειοθέτηση στοιχείων στο γραμματοκιβώτιο αρχειοθέτησης. Βεβαιωθείτε ότι έχετε εκτελέσει τα παρακάτω βήματα:
  
1. Επιβεβαιώστε ότι μια **Αρχειοθέτηση γραμματοκιβώτιο** έχει ενεργοποιηθεί. Εάν όχι, χρησιμοποιήστε τα βήματα σε [αυτό το άρθρο](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) , για να ενεργοποιήσετε το γραμματοκιβώτιο αρχειοθέτησης. 
    
2. Στο Κέντρο διαχείρισης Exchange, επιλέξτε **Ετικέτες διατήρησης** στην περιοχή **Διαχείριση συμμόρφωσης**, δημιουργήστε μια **ετικέτα διατήρησης** με την ενέργεια **μετακινήσετε σε αρχείο αρχειοθέτησης** που περιέχει την επιθυμητή **Ηλικία διατήρησης**.
    
3. Στο Κέντρο διαχείρισης Exchange, επιλέξτε **Πολιτικές διατήρησης**, δημιουργήστε μια **Πολιτική διατήρησης** και προσθέστε την ετικέτα διατήρησης **προς φύλαξη** συγκεκριμένη πολιτική. 
    
4. [Εκχώρηση της πολιτικής διατήρησης](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) στο γραμματοκιβώτιο του συγκεκριμένου χρήστη. Την ίδια πολιτική θα εφαρμοστεί για το **πρωτεύον** και το γραμματοκιβώτιο **αρχειοθέτησης** . 
    
Το γραμματοκιβώτιο του χρήστη θα πρέπει τώρα να έχετε μια πολιτική αρχειοθέτησης για τη μετακίνηση στοιχείων στο γραμματοκιβώτιο αρχειοθέτησης. Μπορεί να είναι απαραίτητο για να εξαναγκαστεί διαχειριζόμενη φάκελο Βοηθός (ΣΠΙ) για να εκτελέσετε και να εφαρμόσετε τις νέες ρυθμίσεις για το γραμματοκιβώτιο του χρήστη. Εκτελέστε την ακόλουθη εντολή ενώ [συνδεδεμένοι EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) για να ξεκινήσετε τη Διαχείριση Βοηθός φακέλου για ένα συγκεκριμένο γραμματοκιβώτιο: 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

Θέλετε περισσότερες πληροφορίες σχετικά με τη διαμόρφωση πολιτικής αρχειοθέτησης, ανατρέξτε στο θέμα [Ρύθμιση μιας πολιτικής αρχειοθέτησης και διαγραφής για τα γραμματοκιβώτια](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  

