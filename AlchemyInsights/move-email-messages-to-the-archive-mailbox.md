---
title: Μετακίνηση μηνυμάτων ηλεκτρονικού ταχυδρομείου στο γραμματοκιβώτιο αρχειοθέτησης
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
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 61d0b1a58fff6655b745bb9d39e8384f0a543336
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799780"
---
# <a name="move-email-to-the-archive-mailbox"></a>Μετακίνηση ηλεκτρονικού ταχυδρομείου στο γραμματοκιβώτιο αρχειοθέτησης

Εάν θέλετε να εκτελέσουμε αυτοματοποιημένους ελέγχους για τις ρυθμίσεις που αναφέρονται παρακάτω, επιλέξτε το κουμπί πίσω <--στο επάνω μέρος αυτής της σελίδας και, στη συνέχεια, πληκτρολογήστε τη διεύθυνση ηλεκτρονικού ταχυδρομείου του χρήστη που αντιμετωπίζει προβλήματα με τη μετακίνηση ηλεκτρονικού ταχυδρομείου στο γραμματοκιβώτιό του.

1. Επιβεβαιώστε ότι έχει ενεργοποιηθεί ένα **γραμματοκιβώτιο αρχειοθέτησης** . Εάν όχι, χρησιμοποιήστε τα βήματα σε [αυτό το άρθρο](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) για να ενεργοποιήσετε το γραμματοκιβώτιο αρχειοθέτησης.

2. Για να αρχειοθετήσετε μηνύματα αυτόματα στο γραμματοκιβώτιο αρχειοθέτησης, μια ετικέτα διατήρησης με την ενέργεια **Μετακίνηση σε αρχειοθέτηση** πρέπει να είναι ρυθμισμένη ώστε να **εφαρμόζεται αυτόματα σε ολόκληρο το γραμματοκιβώτιο (προεπιλογή)**. Χρησιμοποιήστε τα βήματα εδώ για να δημιουργήσετε την ετικέτα: [Αρχειοθέτηση προεπιλεγμένης ετικέτας](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Στη συνέχεια, προσθέστε την ετικέτα **αρχειοθέτησης** στην πολιτική διατήρησης. Στο κέντρο διαχείρισης του Exchange, επιλέξτε **πολιτικές διατήρησης** > προσθέσετε την **ετικέτα μετακίνηση σε αρχειοθέτηση** στην πολιτική > **Αποθήκευση**.

4. Τώρα, [εκχωρήστε την πολιτική διατήρησης](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) στο γραμματοκιβώτιο του συγκεκριμένου χρήστη. Η ίδια πολιτική θα εφαρμοστεί και στο γραμματοκιβώτιο " **πρωτεύον** " και " **αρχειοθήκη** ".

Ίσως χρειαστεί να αναγκάσετε τον βοηθό διαχειριζόμενου φακέλου (ΣΠΙ) να εκτελέσει και να εφαρμόσει τις νέες ρυθμίσεις στο γραμματοκιβώτιο του χρήστη. Εκτελέστε την ακόλουθη εντολή ενώ [είστε συνδεδεμένοι στο έξω PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) για να ξεκινήσετε τον βοηθό διαχειριζόμενου φακέλου για ένα συγκεκριμένο γραμματοκιβώτιο:
  
Έναρξη-ManagedFolderAssistant-ταυτότητα <name of the mailbox>

Για περισσότερες πληροφορίες σχετικά με τη ρύθμιση μιας πολιτικής αρχειοθέτησης, ανατρέξτε στο θέμα [ρύθμιση πολιτικής αρχειοθέτησης και διαγραφής για τα γραμματοκιβώτια](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  