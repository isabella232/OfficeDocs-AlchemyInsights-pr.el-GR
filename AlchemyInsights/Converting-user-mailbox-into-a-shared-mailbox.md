---
title: Μετατροπή γραμματοκιβώτιο χρήστη σε ένα κοινόχρηστο γραμματοκιβώτιο;
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Normal
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: ab34b8939b95b29bedb797f640dd744bc783adef
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36496399"
---
# <a name="convert-a-user-mail-box-into-a-shared-mailbox"></a>Μετατρέψτε μια θυρίδα αλληλογραφίας του χρήστη σε ένα κοινόχρηστο γραμματοκιβώτιο

Μπορείτε να μετατρέψετε ένα γραμματοκιβώτιο χρήστη σε ένα κοινόχρηστο γραμματοκιβώτιο, μόνο εάν ο χρήστης έχει άδεια χρήσης Exchange. Μετά τη μετατροπή του γραμματοκιβωτίου, θα συνεχίσει να εμφανίζεται στη λίστα ενεργών χρηστών επειδή η λίστα αυτή περιλαμβάνει κοινόχρηστα γραμματοκιβώτια. Ωστόσο, το γραμματοκιβώτιο που έχει μετατραπεί θα εμφανίζει επίσης προς τα επάνω στη λίστα κοινόχρηστο γραμματοκιβώτιο. 
  
Εάν προσπαθείτε να μετατρέψετε ένα γραμματοκιβώτιο στην κονσόλα διαχείρισης του Exchange και η μετατροπή αποτύχει, καταργήστε την cache του προγράμματος περιήγησης και τα cookies και προσπαθήστε ξανά. Εάν ακόμα δεν λειτουργεί, προσπαθήστε να μετατρέψετε το γραμματοκιβώτιο με το κέλυφος διαχείρισης Exchange εκτελώντας την ακόλουθη εντολή:
  
```
Set-Mailbox -Type Shared
```

Περισσότερες πληροφορίες μετατροπής του γραμματοκιβωτίου είναι διαθέσιμη στη [Μετατροπή ενός γραμματοκιβωτίου χρήστη σε ένα κοινόχρηστο γραμματοκιβώτιο](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).
  
