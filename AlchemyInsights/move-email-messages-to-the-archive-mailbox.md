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
ms.openlocfilehash: 37f256ef31402f5139fdd7c2af8f3a6ca9dc3525
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32418310"
---
# <a name="move-email-to-the-archive-mailbox"></a>Μετακίνηση μηνύματος ηλεκτρονικού ταχυδρομείου στο γραμματοκιβώτιο αρχειοθέτησης
 
1. Επιβεβαιώστε ότι μια **Αρχειοθέτηση γραμματοκιβώτιο** έχει ενεργοποιηθεί. Εάν όχι, ακολουθήστε τα βήματα σε [αυτό το άρθρο](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) , για να ενεργοποιήσετε το γραμματοκιβώτιο αρχειοθέτησης.

2. Για να αρχειοθετήσετε μηνύματα αυτόματα στο γραμματοκιβώτιο αρχειοθέτησης, πρέπει να οριστεί μια ετικέτα διατήρησης με την ενέργεια της **μετακίνησης για να αρχειοθετήσετε** εφαρμόζεται **αυτόματα σε tag ολόκληρου του γραμματοκιβωτίου (προεπιλογή)**. Χρησιμοποιήστε εδώ τα βήματα για να δημιουργήσετε το tag: [Αρχειοθέτηση προεπιλεγμένη ετικέτα](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0).
    
3. Στη συνέχεια, προσθέστε την ετικέτα **αρχειοθέτησης** στην πολιτική διατήρησης. Στο Κέντρο διαχείρισης Exchange, επιλέξτε **Πολιτικές διατήρησης** > προσθέσετε **προς φύλαξη tag** για την > πολιτική **Αποθήκευση**. 
    
4. Τώρα την [εκχώρηση της πολιτικής διατήρησης](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) στο γραμματοκιβώτιο του συγκεκριμένου χρήστη. Την ίδια πολιτική θα εφαρμοστεί για το **πρωτεύον** και το γραμματοκιβώτιο **αρχειοθέτησης** . 
    
Μπορεί να είναι απαραίτητο για να εξαναγκαστεί διαχειριζόμενη φάκελο Βοηθός (ΣΠΙ) για να εκτελέσετε και να εφαρμόσετε τις νέες ρυθμίσεις για το γραμματοκιβώτιο του χρήστη. Εκτελέστε την ακόλουθη εντολή ενώ [συνδεδεμένοι EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) για να ξεκινήσετε τη Διαχείριση Βοηθός φακέλου για ένα συγκεκριμένο γραμματοκιβώτιο: 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

Για περισσότερες πληροφορίες σχετικά με τη δημιουργία μιας πολιτικής αρχειοθέτησης, ανατρέξτε στο θέμα [Ρύθμιση μιας πολιτικής αρχειοθέτησης και διαγραφής για τα γραμματοκιβώτια](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  

