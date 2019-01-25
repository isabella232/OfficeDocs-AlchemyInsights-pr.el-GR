---
title: Μετατροπή γραμματοκιβώτιο χρήστη σε ένα κοινόχρηστο γραμματοκιβώτιο;
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Priority
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: 22ad1b3fb818b40bcd77974031735f931e986968
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29470956"
---
<span data-ttu-id="91b34-p101">Μπορείτε να μετατρέψετε ένα γραμματοκιβώτιο χρήστη σε ένα κοινόχρηστο γραμματοκιβώτιο, μόνο εάν ο χρήστης έχει άδεια χρήσης Exchange. Μετά τη μετατροπή του γραμματοκιβωτίου, θα συνεχίσει να εμφανίζεται στη λίστα ενεργών χρηστών επειδή η λίστα αυτή περιλαμβάνει κοινόχρηστα γραμματοκιβώτια. Ωστόσο, το γραμματοκιβώτιο που έχει μετατραπεί θα εμφανίζει επίσης προς τα επάνω στη λίστα κοινόχρηστο γραμματοκιβώτιο.</span><span class="sxs-lookup"><span data-stu-id="91b34-p101">You can only convert a user mailbox to a shared mailbox if the user has an Exchange license. After the mailbox is converted, it will continue to show up in the active users list because that list includes shared mailboxes. However, the converted mailbox will also show up in the shared mailbox list.</span></span> 
  
<span data-ttu-id="91b34-p102">Εάν προσπαθείτε να μετατρέψετε ένα γραμματοκιβώτιο στην κονσόλα διαχείρισης του Exchange και η μετατροπή αποτύχει, καταργήστε την cache του προγράμματος περιήγησης και τα cookies και προσπαθήστε ξανά. Εάν ακόμα δεν λειτουργεί, προσπαθήστε να μετατρέψετε το γραμματοκιβώτιο με το κέλυφος διαχείρισης Exchange εκτελώντας την ακόλουθη εντολή:</span><span class="sxs-lookup"><span data-stu-id="91b34-p102">If you try to convert a mailbox in the Exchange Admin Console and the conversion fails, clear your browser cache and cookies and try again. If it still isn't working, try converting the mailbox in the Exchange Management Shell by running the following command:</span></span>
  
```
Set-Mailbox -Type Shared
```

<span data-ttu-id="91b34-107">Περισσότερες πληροφορίες μετατροπής του γραμματοκιβωτίου είναι διαθέσιμη στη [Μετατροπή ενός γραμματοκιβωτίου χρήστη σε ένα κοινόχρηστο γραμματοκιβώτιο](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span><span class="sxs-lookup"><span data-stu-id="91b34-107">More mailbox conversion information is available in [Convert a user mailbox to a shared mailbox](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span></span>
  
