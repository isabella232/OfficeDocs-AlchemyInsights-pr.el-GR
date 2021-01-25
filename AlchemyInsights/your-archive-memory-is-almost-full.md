---
title: Το γραμματοκιβώτιο αρχειοθέτησης είναι σχεδόν πλήρες
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 5c7081f8991716a8ac72f462c6c7ef88e800ab9c
ms.sourcegitcommit: 6f1af4aed507d4c074c36d77666cf00100efe168
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974403"
---
# <a name="your-archive-mailbox-is-almost-full"></a>Το γραμματοκιβώτιο αρχειοθέτησης είναι σχεδόν πλήρες

Εάν ο χρήστης λάβει την προειδοποίηση, **Το γραμματοκιβώτιο αρχειοθέτησης είναι σχεδόν πλήρες** ή πρέπει να αυξήσετε το μέγεθος του γραμματοκιβωτίου αρχειοθέτησης, ακολουθούν ορισμένες συμβουλές:

1. Εάν ο χρήστης έχει αντιστοιχιστεί σε ένα πρόγραμμα Exchange Online 1, κάντε αναβάθμιση στην άδεια χρήσης του **Exchange Online Plan 2** για να αυξήσετε το μέγεθος από το 50 GB στο 100GB.
1. Εάν ο χρήστης έχει ήδη εκχωρηθεί ένα από τα εξής: **Exchange Online Plan 2** ή ένα Exchange Online πρόγραμμα 1 με ένα πρόσθετο αρχειοθέτησης του Exchange Online, χρησιμοποιήστε τα παρακάτω βήματα για να ενεργοποιήσετε την αυτόματη επέκταση της αρχειοθέτησης:.
 
    1. [Σύνδεση στο Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).
    2. Εκτελέστε τα παρακάτω commandlet για το χρήστη:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. Εκτελέστε το ακόλουθο commandlet για να επιβεβαιώσετε ότι έχει ενεργοποιηθεί για το χρήστη:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

Για περισσότερες πληροφορίες, ανατρέξτε στα θέματα:

- [ Ενεργοποίηση απεριόριστης αρχειοθέτησης-βοήθεια για διαχειριστές-συμμόρφωση της Microsoft 365 | Έγγραφα της Microsoft](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Όρια του Exchange Online-περιγραφές υπηρεσιών | Έγγραφα της Microsoft](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [Αναβάθμιση σε διαφορετικό επιχειρηματικό σχέδιο | Έγγραφα της Microsoft](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

