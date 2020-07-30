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
ms.openlocfilehash: 9af8a4d3ce72fd901ff2f3a1aae0654c7213dd7e
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522771"
---
# <a name="move-email-to-the-archive-mailbox"></a>Μετακίνηση ηλεκτρονικού ταχυδρομείου στο γραμματοκιβώτιο αρχειοθέτησης

Αν θέλετε να εκτελέσουμε αυτοματοποιημένους ελέγχους για τις ρυθμίσεις που αναφέρονται παρακάτω, επιλέξτε το κουμπί "Πίσω" <-- στο επάνω μέρος αυτής της σελίδας και, στη συνέχεια, πληκτρολογήστε τη διεύθυνση ηλεκτρονικού ταχυδρομείου του χρήστη που αντιμετωπίζει προβλήματα με τη μετακίνηση ηλεκτρονικού ταχυδρομείου στο γραμματοκιβώτιο αρχειοθέτησης.

1. Επιβεβαιώστε ότι έχει ενεργοποιηθεί ένα **γραμματοκιβώτιο αρχειοθέτησης.** Εάν όχι, χρησιμοποιήστε τα βήματα [αυτού του άρθρου](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) για να ενεργοποιήσετε το γραμματοκιβώτιο αρχειοθέτησης.

2. Για να αρχειοθετηθούν αυτόματα τα μηνύματα στο γραμματοκιβώτιο αρχειοθέτησης, μια ετικέτα διατήρησης με την ενέργεια **Μετακίνηση στην αρχειοθέτηση** πρέπει να ρυθμιστεί ώστε να **εφαρμόζεται αυτόματα σε ολόκληρο το γραμματοκιβώτιο (προεπιλεγμένο) tag**. Χρησιμοποιήστε τα βήματα εδώ για να δημιουργήσετε την ετικέτα: [Αρχειοθέτηση προεπιλεγμένη ετικέτα](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Στη συνέχεια, προσθέστε την ετικέτα **Αρχειοθέτηση** στην πολιτική διατήρησης. Στο κέντρο διαχείρισης του Exchange, επιλέξτε **Πολιτικές διατήρησης** > προσθέστε την **ετικέτα Μετακίνηση στην αρχειοθέτηση** στην πολιτική > **Αποθήκευση**.

4. Τώρα [αντιστοιχίστε την πολιτική διατήρησης](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) στο γραμματοκιβώτιο του συγκεκριμένου χρήστη. Η ίδια πολιτική θα εφαρμοστεί τόσο στο **γραμματοκιβώτιο "Κύρια"** όσο και στο γραμματοκιβώτιο **"Αρχειοθέτηση".**

Ίσως χρειαστεί να επιβάλετε την εκτέλεση και την εφαρμογή των νέων ρυθμίσεων από το Βοηθό διαχειριζόμενων φακέλων (MFA) και να εφαρμόσετε τις νέες ρυθμίσεις στο γραμματοκιβώτιο του χρήστη. Εκτελέστε την ακόλουθη εντολή ενώ [είστε συνδεδεμένοι στο EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) για να ξεκινήσετε το Βοηθό διαχειριζόμενων φακέλων για ένα συγκεκριμένο γραμματοκιβώτιο:
  
Αρχή-Διαχειριζόμενη ΠτυχήAssistant -Ταυτότητα<name of the mailbox>

Για περισσότερες πληροφορίες σχετικά με τη ρύθμιση μιας πολιτικής αρχειοθέτησης, ανατρέξτε στο θέμα [Ρύθμιση πολιτικής αρχειοθέτησης και διαγραφής για γραμματοκιβώτια](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  