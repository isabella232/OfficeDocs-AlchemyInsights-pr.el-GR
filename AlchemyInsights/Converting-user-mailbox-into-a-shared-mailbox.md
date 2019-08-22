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
# <a name="convert-a-user-mail-box-into-a-shared-mailbox"></a><span data-ttu-id="4148b-102">Μετατρέψτε μια θυρίδα αλληλογραφίας του χρήστη σε ένα κοινόχρηστο γραμματοκιβώτιο</span><span class="sxs-lookup"><span data-stu-id="4148b-102">Convert a user mail box into a shared mailbox</span></span>

<span data-ttu-id="4148b-103">Μπορείτε να μετατρέψετε ένα γραμματοκιβώτιο χρήστη σε ένα κοινόχρηστο γραμματοκιβώτιο, μόνο εάν ο χρήστης έχει άδεια χρήσης Exchange.</span><span class="sxs-lookup"><span data-stu-id="4148b-103">You can only convert a user mailbox to a shared mailbox if the user has an Exchange license.</span></span> <span data-ttu-id="4148b-104">Μετά τη μετατροπή του γραμματοκιβωτίου, θα συνεχίσει να εμφανίζεται στη λίστα ενεργών χρηστών επειδή η λίστα αυτή περιλαμβάνει κοινόχρηστα γραμματοκιβώτια.</span><span class="sxs-lookup"><span data-stu-id="4148b-104">After the mailbox is converted, it will continue to show up in the active users list because that list includes shared mailboxes.</span></span> <span data-ttu-id="4148b-105">Ωστόσο, το γραμματοκιβώτιο που έχει μετατραπεί θα εμφανίζει επίσης προς τα επάνω στη λίστα κοινόχρηστο γραμματοκιβώτιο.</span><span class="sxs-lookup"><span data-stu-id="4148b-105">However, the converted mailbox will also show up in the shared mailbox list.</span></span> 
  
<span data-ttu-id="4148b-106">Εάν προσπαθείτε να μετατρέψετε ένα γραμματοκιβώτιο στην κονσόλα διαχείρισης του Exchange και η μετατροπή αποτύχει, καταργήστε την cache του προγράμματος περιήγησης και τα cookies και προσπαθήστε ξανά.</span><span class="sxs-lookup"><span data-stu-id="4148b-106">If you try to convert a mailbox in the Exchange Admin Console and the conversion fails, clear your browser cache and cookies and try again.</span></span> <span data-ttu-id="4148b-107">Εάν ακόμα δεν λειτουργεί, προσπαθήστε να μετατρέψετε το γραμματοκιβώτιο με το κέλυφος διαχείρισης Exchange εκτελώντας την ακόλουθη εντολή:</span><span class="sxs-lookup"><span data-stu-id="4148b-107">If it still isn't working, try converting the mailbox in the Exchange Management Shell by running the following command:</span></span>
  
```
Set-Mailbox -Type Shared
```

<span data-ttu-id="4148b-108">Περισσότερες πληροφορίες μετατροπής του γραμματοκιβωτίου είναι διαθέσιμη στη [Μετατροπή ενός γραμματοκιβωτίου χρήστη σε ένα κοινόχρηστο γραμματοκιβώτιο](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).</span><span class="sxs-lookup"><span data-stu-id="4148b-108">More mailbox conversion information is available in [Convert a user mailbox to a shared mailbox](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).</span></span>
  
