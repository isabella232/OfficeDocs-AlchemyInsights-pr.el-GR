---
title: Ανάκτηση διαγραμμένων στοιχείων με cmdlet
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800008"
- "5718"
ms.openlocfilehash: d8f2a50f39d7bcd321692ab093e2efa6613e9814
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835811"
---
# <a name="recover-deleted-items-with-cmdlet"></a><span data-ttu-id="cee5f-102">Ανάκτηση διαγραμμένων στοιχείων με cmdlet</span><span class="sxs-lookup"><span data-stu-id="cee5f-102">Recover deleted items with cmdlet</span></span>

- <span data-ttu-id="cee5f-103">Χρησιμοποιήστε το [cmdlet Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) για να προβάλετε διαγραμμένα στοιχεία σε γραμματοκιβώτια.</span><span class="sxs-lookup"><span data-stu-id="cee5f-103">Use the [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) cmdlet to view deleted items in mailboxes.</span></span> <span data-ttu-id="cee5f-104">Αφού βρείτε τα διαγραμμένα στοιχεία, μπορείτε να χρησιμοποιήσετε το [cmdlet Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) για να τα επαναφέρετε.</span><span class="sxs-lookup"><span data-stu-id="cee5f-104">After you find the deleted items, you use the [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) cmdlet to restore them.</span></span>

- <span data-ttu-id="cee5f-105">Δείτε τις πλήρεις λεπτομέρειες [στο Get-RecoverableItems.](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="cee5f-105">See full details in [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span></span>

- <span data-ttu-id="cee5f-106">Πρέπει να σας εκχωρηθεί ο ρόλος "Εξαγωγή εισαγωγής γραμματοκιβωτίου" για να μπορείτε να εκτελέσετε αυτό το cmdlet.</span><span class="sxs-lookup"><span data-stu-id="cee5f-106">You need to be assigned the Mailbox Import Export role before you can run this cmdlet.</span></span> <span data-ttu-id="cee5f-107">Ανατρέξτε [στο θέμα Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) για περισσότερες πληροφορίες.</span><span class="sxs-lookup"><span data-stu-id="cee5f-107">Please see [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) for more information.</span></span>
