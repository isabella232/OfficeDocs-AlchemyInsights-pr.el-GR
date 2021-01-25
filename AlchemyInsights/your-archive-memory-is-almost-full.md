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
# <a name="your-archive-mailbox-is-almost-full"></a><span data-ttu-id="4bdde-102">Το γραμματοκιβώτιο αρχειοθέτησης είναι σχεδόν πλήρες</span><span class="sxs-lookup"><span data-stu-id="4bdde-102">Your archive mailbox is almost full</span></span>

<span data-ttu-id="4bdde-103">Εάν ο χρήστης λάβει την προειδοποίηση, **Το γραμματοκιβώτιο αρχειοθέτησης είναι σχεδόν πλήρες** ή πρέπει να αυξήσετε το μέγεθος του γραμματοκιβωτίου αρχειοθέτησης, ακολουθούν ορισμένες συμβουλές:</span><span class="sxs-lookup"><span data-stu-id="4bdde-103">If the user receives the warning; **Your archive mailbox is almost full**, or you need to increase the size of their archive mailbox, here are some tips:</span></span>

1. <span data-ttu-id="4bdde-104">Εάν ο χρήστης έχει αντιστοιχιστεί σε ένα πρόγραμμα Exchange Online 1, κάντε αναβάθμιση στην άδεια χρήσης του **Exchange Online Plan 2** για να αυξήσετε το μέγεθος από το 50 GB στο 100GB.</span><span class="sxs-lookup"><span data-stu-id="4bdde-104">If the user is assigned an Exchange Online Plan 1, upgrade to **Exchange Online Plan 2** license to increase the size from 50 GB to 100GB.</span></span>
1. <span data-ttu-id="4bdde-105">Εάν ο χρήστης έχει ήδη εκχωρηθεί ένα από τα εξής: **Exchange Online Plan 2** ή ένα Exchange Online πρόγραμμα 1 με ένα πρόσθετο αρχειοθέτησης του Exchange Online, χρησιμοποιήστε τα παρακάτω βήματα για να ενεργοποιήσετε την αυτόματη επέκταση της αρχειοθέτησης:.</span><span class="sxs-lookup"><span data-stu-id="4bdde-105">If the user is already assigned either of the following: **Exchange Online Plan 2** or an Exchange Online Plan 1 with an Exchange Online Archiving add-on, use the steps below to enable Auto-Expanding archiving:.</span></span>
 
    1. <span data-ttu-id="4bdde-106">[Σύνδεση στο Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="4bdde-106">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).</span></span>
    2. <span data-ttu-id="4bdde-107">Εκτελέστε τα παρακάτω commandlet για το χρήστη:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span><span class="sxs-lookup"><span data-stu-id="4bdde-107">Run the following commandlet for the user:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span></span>
    1. <span data-ttu-id="4bdde-108">Εκτελέστε το ακόλουθο commandlet για να επιβεβαιώσετε ότι έχει ενεργοποιηθεί για το χρήστη:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span><span class="sxs-lookup"><span data-stu-id="4bdde-108">Run the following commandlet to confirm it is enabled for the user:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span></span>

<span data-ttu-id="4bdde-109">Για περισσότερες πληροφορίες, ανατρέξτε στα θέματα:</span><span class="sxs-lookup"><span data-stu-id="4bdde-109">For more information see:</span></span>

- [<span data-ttu-id="4bdde-110"> Ενεργοποίηση απεριόριστης αρχειοθέτησης-βοήθεια για διαχειριστές-συμμόρφωση της Microsoft 365 | Έγγραφα της Microsoft</span><span class="sxs-lookup"><span data-stu-id="4bdde-110"> Enable unlimited archiving - Admin Help - Microsoft 365 Compliance | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [<span data-ttu-id="4bdde-111">Όρια του Exchange Online-περιγραφές υπηρεσιών | Έγγραφα της Microsoft</span><span class="sxs-lookup"><span data-stu-id="4bdde-111">Exchange Online limits - Service Descriptions | Microsoft Docs</span></span>](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [<span data-ttu-id="4bdde-112">Αναβάθμιση σε διαφορετικό επιχειρηματικό σχέδιο | Έγγραφα της Microsoft</span><span class="sxs-lookup"><span data-stu-id="4bdde-112">Upgrade to a different business plan | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

