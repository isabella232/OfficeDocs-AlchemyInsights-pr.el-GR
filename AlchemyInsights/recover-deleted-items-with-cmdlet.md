---
title: Ανάκτηση διαγραμμένων στοιχείων με cmdlet
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800008"
- "5718"
ms.openlocfilehash: 86744d92a44096991079d1da3bdf4e95e58c55b7
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 05/26/2020
ms.locfileid: "44493025"
---
# <a name="recover-deleted-items-with-cmdlet"></a><span data-ttu-id="d4893-102">Ανάκτηση διαγραμμένων στοιχείων με cmdlet</span><span class="sxs-lookup"><span data-stu-id="d4893-102">Recover deleted items with cmdlet</span></span>

- <span data-ttu-id="d4893-103">Χρησιμοποιήστε το cmdlet [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) για να προβάλετε διαγραμμένα στοιχεία σε γραμματοκιβώτια.</span><span class="sxs-lookup"><span data-stu-id="d4893-103">Use the [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) cmdlet to view deleted items in mailboxes.</span></span> <span data-ttu-id="d4893-104">Αφού βρείτε τα διαγραμμένα στοιχεία, μπορείτε να χρησιμοποιήσετε το cmdlet [Επαναφορά-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) για να τα επαναφέρετε.</span><span class="sxs-lookup"><span data-stu-id="d4893-104">After you find the deleted items, you use the [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) cmdlet to restore them.</span></span>

- <span data-ttu-id="d4893-105">Δείτε όλες τις λεπτομέρειες στο [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="d4893-105">See full details in [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span></span>

- <span data-ttu-id="d4893-106">Πρέπει να σας ανατεθεί ο ρόλος εξαγωγής εισαγωγής γραμματοκιβωτίου για να μπορέσετε να εκτελέσετε αυτό το cmdlet.</span><span class="sxs-lookup"><span data-stu-id="d4893-106">You need to be assigned the Mailbox Import Export role before you can run this cmdlet.</span></span> <span data-ttu-id="d4893-107">Ανατρέξτε στην [προπαρασενία Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) για περισσότερες πληροφορίες.</span><span class="sxs-lookup"><span data-stu-id="d4893-107">Please see [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) for more information.</span></span>
