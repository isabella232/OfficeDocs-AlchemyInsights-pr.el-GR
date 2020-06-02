---
title: Μετακίνηση μηνυμάτων ηλεκτρονικού ταχυδρομείου στο γραμματοκιβώτιο αρχειοθέτησης
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 35c11f1bfb7c61b28a64f0128c29ddf7b4fce939
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511040"
---
# <a name="move-email-to-the-archive-mailbox"></a>Μετακίνηση ηλεκτρονικού ταχυδρομείου στο γραμματοκιβώτιο αρχειοθέτησης

1. Επιβεβαιώστε ότι έχει ενεργοποιηθεί ένα **γραμματοκιβώτιο αρχειοθέτησης.** Εάν όχι, χρησιμοποιήστε τα βήματα αυτού του [άρθρου](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) για να ενεργοποιήσετε το γραμματοκιβώτιο αρχειοθέτησης.

2. Για να αρχειοθετήσετε μηνύματα αυτόματα στο γραμματοκιβώτιο αρχειοθέτησης, πρέπει να οριστεί μια ετικέτα διατήρησης με την ενέργεια **Μετακίνηση στην αρχειοθέτηση,** ώστε **να εφαρμόζεται αυτόματα σε ολόκληρη την ετικέτα γραμματοκιβωτίου (προεπιλογή).** Χρησιμοποιήστε τα βήματα εδώ για να δημιουργήσετε την ετικέτα: [Αρχειοθέτηση προεπιλεγμένη ετικέτα](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Στη συνέχεια, προσθέστε την ετικέτα **Αρχειοθέτηση** στην πολιτική διατήρησης. Στο κέντρο διαχείρισης του Exchange, επιλέξτε **Πολιτικές διατήρησης** > προσθέσετε την **ετικέτα Μετακίνηση στην αρχειοθέτηση** στην πολιτική > **Αποθήκευση**.

4. Τώρα [Αντιστοιχίστε την πολιτική διατήρησης](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) στο γραμματοκιβώτιο του συγκεκριμένου χρήστη. Η ίδια πολιτική θα εφαρμοστεί τόσο στο **γραμματοκιβώτιο "Κύρια"** όσο και στο γραμματοκιβώτιο **αρχειοθέτησης.**

Ίσως χρειαστεί να επιβάλετε την εκτέλεση του Βοηθού διαχειριζόμενου φακέλου (MFA) και να εφαρμόσετε τις νέες ρυθμίσεις στο γραμματοκιβώτιο του χρήστη. Εκτελέστε την ακόλουθη εντολή ενώ [είστε συνδεδεμένοι στο EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) για να ξεκινήσετε το Βοηθό διαχειριζόμενου φακέλου για ένα συγκεκριμένο γραμματοκιβώτιο:
  
Start-ManagedFolderAssistant -Ταυτότητα<name of the mailbox>

Για περισσότερες πληροφορίες σχετικά με τη ρύθμιση μιας πολιτικής [αρχειοθέτησης, ανατρέξτε στο θέμα Ρύθμιση πολιτικής αρχειοθέτησης και διαγραφής για γραμματοκιβώτια](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  