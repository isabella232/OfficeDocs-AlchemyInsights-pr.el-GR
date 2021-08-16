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
ms.openlocfilehash: 085d9b211d5a8e9a0e1eb12af14d87a4e59c844a3afa012095dfd60db316ad14
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046752"
---
# <a name="your-archive-mailbox-is-almost-full"></a>Το γραμματοκιβώτιο αρχειοθέτησης είναι σχεδόν πλήρες

Εάν ο χρήστης λάβει την προειδοποίηση, **Το γραμματοκιβώτιο αρχειοθέτησης είναι σχεδόν πλήρες** ή πρέπει να αυξήσετε το μέγεθος του γραμματοκιβωτίου αρχειοθήκης, ακολουθούν ορισμένες συμβουλές:

1. Εάν στο χρήστη έχει εκχωρηθεί ένα πρόγραμμα Exchange Online 1, αναβαθμίστε σε **Exchange Online Πρόγραμμα 2** για να αυξήσετε το μέγεθος από 50 GB σε 100 GB.
1. Εάν στο χρήστη έχει ήδη εκχωρηθεί ένα από τα εξής: Exchange Online Πρόγραμμα **2** ή πρόγραμμα Exchange Online 1 με πρόσθετο του Αρχειοθέτηση Exchange Online, ακολουθήστε τα παρακάτω βήματα για να ενεργοποιήσετε την αυτόματη ανάπτυξη αρχειοθέτησης:.
 
    1. [Σύνδεση να Exchange Online Powershell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true)
    2. Εκτελέστε το ακόλουθο commandlet για το χρήστη:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. Εκτελέστε το ακόλουθο commandlet για να επιβεβαιώσετε ότι είναι ενεργοποιημένο για το χρήστη:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα:

- [Ενεργοποίηση απεριόριστης αρχειοθέτησης - Βοήθεια για διαχειριστές - Microsoft 365 συμμόρφωσης | Microsoft Docs](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Exchange Online όρια - Περιγραφές υπηρεσίας | Microsoft Docs](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [Αναβάθμιση σε διαφορετικό πρόγραμμα | Microsoft Docs](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

