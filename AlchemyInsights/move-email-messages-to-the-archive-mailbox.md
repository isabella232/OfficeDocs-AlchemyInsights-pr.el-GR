---
title: Μετακίνηση μηνυμάτων ηλεκτρονικού ταχυδρομείου στο γραμματοκιβώτιο αρχειοθέτησης
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 5592bc7d4566e3498c33bbf9488db7f46ec58842
ms.sourcegitcommit: 8864b5789d9905916039081b53530c7e6d8bc529
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822162"
---
# <a name="move-email-to-the-archive-mailbox"></a>Μετακίνηση ηλεκτρονικού ταχυδρομείου στο γραμματοκιβώτιο αρχειοθέτησης

1. Επιβεβαιώστε ότι έχει ενεργοποιηθεί ένα **γραμματοκιβώτιο αρχειοθέτησης** . Εάν όχι, χρησιμοποιήστε τα βήματα [αυτού του άρθρου](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) για να ενεργοποιήσετε το γραμματοκιβώτιο αρχειοθέτησης.

2. Για να αρχειοθετήσετε μηνύματα αυτόματα στο γραμματοκιβώτιο αρχειοθέτησης, μια ετικέτα διατήρησης με το **Move για την αρχειοθέτηση** ενέργειας πρέπει να οριστεί να **εφαρμοστεί αυτόματα σε ολόκληρη την ετικέτα γραμματοκιβωτίου (προεπιλογή)**. Χρησιμοποιήστε τα βήματα εδώ για να δημιουργήσετε την ετικέτα: [Αρχειοθέτηση προεπιλεγμένη ετικέτα](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Στη συνέχεια, προσθέστε την ετικέτα **αρχειοθέτησης** στην πολιτική διατήρησης. Στο κέντρο διαχείρισης του Exchange, επιλέξτε **πολιτικές διατήρησης** > προσθέσετε την **ετικέτα μετακίνηση στην αρχειοθέτηση** στην πολιτική > **Αποθήκευση**.

4. Τώρα [Αντιστοιχίστε την πολιτική διατήρησης](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) στο γραμματοκιβώτιο του συγκεκριμένου χρήστη. Η ίδια πολιτική θα εφαρμοστεί τόσο στο **πρωτεύον** όσο και στο γραμματοκιβώτιο **αρχειοθέτησης** .

Μπορεί να είναι απαραίτητο να επιβάλετε το διαχειριζόμενο βοηθό φακέλου (ΣΠΙ) για να εκτελέσετε και να εφαρμόσετε τις νέες ρυθμίσεις στο γραμματοκιβώτιο του χρήστη. Εκτελέστε την ακόλουθη εντολή, ενώ έχετε [συνδεθεί με έξω PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) για να ξεκινήσετε το διαχειριζόμενο βοηθό φακέλου για ένα συγκεκριμένο γραμματοκιβώτιο:
  
Βοηθός φακέλου-αρχή διαχείρισης-ταυτότητα<name of the mailbox>

Για περισσότερες πληροφορίες σχετικά με τη ρύθμιση μιας πολιτικής αρχειοθέτησης, ανατρέξτε στο στοιχείο [ρύθμιση πολιτικής αρχειοθέτησης και διαγραφής για γραμματοκιβώτια](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  