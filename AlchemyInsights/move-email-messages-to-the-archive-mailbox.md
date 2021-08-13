---
title: Μετακίνηση μηνυμάτων ηλεκτρονικού ταχυδρομείου στο γραμματοκιβώτιο αρχειοθήκης
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
ms.openlocfilehash: 7e72766f441e210a81fcfd6c07b1801f6c0474afb02a70edf2ad8dbb571f3d2a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53974957"
---
# <a name="move-email-to-the-archive-mailbox"></a>Μετακίνηση ηλεκτρονικού ταχυδρομείου στο γραμματοκιβώτιο αρχειοθέτησης

Εάν θέλετε να εκτελέσουμε αυτοματοποιημένους ελέγχους για τις ρυθμίσεις που αναφέρονται παρακάτω, επιλέξτε το κουμπί "Πίσω" <-- στο επάνω μέρος αυτής της σελίδας και, στη συνέχεια, πληκτρολογήστε τη διεύθυνση ηλεκτρονικού ταχυδρομείου του χρήστη που έχει προβλήματα μετακίνησης ηλεκτρονικού ταχυδρομείου στο γραμματοκιβώτιο αρχειοθέτησης.

1. Επιβεβαιώστε ότι **έχει ενεργοποιηθεί ένα** γραμματοκιβώτιο αρχειοθήκης. Εάν όχι, ακολουθήστε τα βήματα σε αυτό το [άρθρο για να](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) ενεργοποιήσετε το γραμματοκιβώτιο αρχειοθέτησης.

2. Για αυτόματη αρχειοθέτηση μηνυμάτων στο γραμματοκιβώτιο αρχειοθέτησης, πρέπει να οριστεί μια ετικέτα διατήρησης με την ενέργεια "Μετακίνηση σε αρχειοθέτηση" ώστε να εφαρμόζεται αυτόματα σε **ολόκληρο το γραμματοκιβώτιο (προεπιλογή).**  Ακολουθήστε τα βήματα εδώ για να δημιουργήσετε την ετικέτα: [Προεπιλεγμένη ετικέτα αρχειοθέτησης.](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag)

3. Στη συνέχεια, προσθέστε την **ετικέτα Αρχειοθήκη** στην πολιτική διατήρησης. Στο κέντρο διαχείρισης Exchange, επιλέξτε  "Πολιτικές διατήρησης" > προσθέσετε την ετικέτα **"Μετακίνηση** στην αρχειοθήκη" στην πολιτική > **"Αποθήκευση".**

4. Τώρα, [αντιστοιχίστε την πολιτική](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) διατήρησης στο γραμματοκιβώτιο του συγκεκριμένου χρήστη. Η ίδια πολιτική θα εφαρμοστεί τόσο στο κύριο όσο **και** στο γραμματοκιβώτιο **αρχειοθήκης.**

Ίσως χρειαστεί να επιβάλετε την εκτέλεση του Βοηθού διαχειριζόμενων φακέλων (MFA) και την εφαρμογή των νέων ρυθμίσεων στο γραμματοκιβώτιο του χρήστη. Εκτελέστε την ακόλουθη εντολή ενώ [είστε συνδεδεμένοι στο EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) για να ξεκινήσετε τον Βοηθό διαχειριζόμενων φακέλων για ένα συγκεκριμένο γραμματοκιβώτιο:
  
Start-ManagedFolderAssistant -Identity <name of the mailbox>

Για περισσότερες πληροφορίες σχετικά με τη ρύθμιση μιας πολιτικής αρχειοθέτησης, ανατρέξτε στο θέμα [Ρύθμιση πολιτικής αρχειοθέτησης και διαγραφής για γραμματοκιβώτια.](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)
  