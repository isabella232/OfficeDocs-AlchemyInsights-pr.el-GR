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
ms.openlocfilehash: 4da54121763fd33aa111f3bb3c26963cd271dc51
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32374323"
---
<span data-ttu-id="449a9-102">Μπορείτε να μετατρέψετε ένα γραμματοκιβώτιο χρήστη σε ένα κοινόχρηστο γραμματοκιβώτιο, μόνο εάν ο χρήστης έχει άδεια χρήσης Exchange.</span><span class="sxs-lookup"><span data-stu-id="449a9-102">You can only convert a user mailbox to a shared mailbox if the user has an Exchange license.</span></span> <span data-ttu-id="449a9-103">Μετά τη μετατροπή του γραμματοκιβωτίου, θα συνεχίσει να εμφανίζεται στη λίστα ενεργών χρηστών επειδή η λίστα αυτή περιλαμβάνει κοινόχρηστα γραμματοκιβώτια.</span><span class="sxs-lookup"><span data-stu-id="449a9-103">After the mailbox is converted, it will continue to show up in the active users list because that list includes shared mailboxes.</span></span> <span data-ttu-id="449a9-104">Ωστόσο, το γραμματοκιβώτιο που έχει μετατραπεί θα εμφανίζει επίσης προς τα επάνω στη λίστα κοινόχρηστο γραμματοκιβώτιο.</span><span class="sxs-lookup"><span data-stu-id="449a9-104">However, the converted mailbox will also show up in the shared mailbox list.</span></span> 
  
<span data-ttu-id="449a9-105">Εάν προσπαθείτε να μετατρέψετε ένα γραμματοκιβώτιο στην κονσόλα διαχείρισης του Exchange και η μετατροπή αποτύχει, καταργήστε την cache του προγράμματος περιήγησης και τα cookies και προσπαθήστε ξανά.</span><span class="sxs-lookup"><span data-stu-id="449a9-105">If you try to convert a mailbox in the Exchange Admin Console and the conversion fails, clear your browser cache and cookies and try again.</span></span> <span data-ttu-id="449a9-106">Εάν ακόμα δεν λειτουργεί, προσπαθήστε να μετατρέψετε το γραμματοκιβώτιο με το κέλυφος διαχείρισης Exchange εκτελώντας την ακόλουθη εντολή:</span><span class="sxs-lookup"><span data-stu-id="449a9-106">If it still isn't working, try converting the mailbox in the Exchange Management Shell by running the following command:</span></span>
  
```
Set-Mailbox -Type Shared
```

<span data-ttu-id="449a9-107">Περισσότερες πληροφορίες μετατροπής του γραμματοκιβωτίου είναι διαθέσιμη στη [Μετατροπή ενός γραμματοκιβωτίου χρήστη σε ένα κοινόχρηστο γραμματοκιβώτιο](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span><span class="sxs-lookup"><span data-stu-id="449a9-107">More mailbox conversion information is available in [Convert a user mailbox to a shared mailbox](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span></span>
  
