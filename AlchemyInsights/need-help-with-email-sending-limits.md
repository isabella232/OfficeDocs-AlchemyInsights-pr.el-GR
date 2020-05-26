---
title: Χρειάζεστε βοήθεια με τα όρια αποστολής μηνυμάτων ηλεκτρονικού ταχυδρομείου;
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: 7f563df313c869d18c3e4240d271c649a74914af
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 05/20/2020
ms.locfileid: "44357548"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="8930d-102">Χρειάζεστε βοήθεια με τα όρια αποστολής μηνυμάτων ηλεκτρονικού ταχυδρομείου;</span><span class="sxs-lookup"><span data-stu-id="8930d-102">Need help with email sending limits?</span></span>

<span data-ttu-id="8930d-103">Παρακάτω είναι τα **όρια αποστολής από το σχεδιασμό** που επιβάλλονται στην υπηρεσία.</span><span class="sxs-lookup"><span data-stu-id="8930d-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="8930d-104">Περισσότερες πληροφορίες σχετικά με αυτά τα όρια τεκμηριώνονται [εδώ](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span><span class="sxs-lookup"><span data-stu-id="8930d-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="8930d-105">Για να αποθαρρύνουμε την παράδοση ανεπιθύμητων μαζικών μηνυμάτων, εφαρμόζουμε όρια χρέωσης παραλήπτη ανά χρήστη **σε όλα τα εξερχόμενα και εσωτερικά μηνύματα**.</span><span class="sxs-lookup"><span data-stu-id="8930d-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="8930d-106">Σε όλες τις SKU, αυτό το όριο είναι **10.000 παραλήπτες ανά ημέρα**.</span><span class="sxs-lookup"><span data-stu-id="8930d-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="8930d-107">Οι πελάτες που πρέπει να στείλουν νόμιμα μαζικά εμπορικά μηνύματα ηλεκτρονικού ταχυδρομείου (για παράδειγμα, ενημερωτικά δελτία πελατών) θα πρέπει να χρησιμοποιούν τρίτους παρόχους που ειδικεύονται σε αυτές τις υπηρεσίες.</span><span class="sxs-lookup"><span data-stu-id="8930d-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="8930d-108">**Σημείωση**: Μόλις συμπληρωθεί το όριο χρέωσης παραλήπτη, δεν είναι δυνατή η αποστολή μηνυμάτων από το γραμματοκιβώτιο μέχρι ο αριθμός των παραληπτών που στάλθηκαν μηνύματα τις τελευταίες 24 ώρες να πέσει κάτω από το όριο.</span><span class="sxs-lookup"><span data-stu-id="8930d-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="8930d-109">Ο χρήστης δεν θα μπορεί να στείλει μηνύματα μέχρι αυτό το σημείο.</span><span class="sxs-lookup"><span data-stu-id="8930d-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="8930d-110">Εφαρμόζεται όριο χρέωσης **μηνυμάτων 30 μηνυμάτων ανά λεπτό** σε όλες τις SKU.</span><span class="sxs-lookup"><span data-stu-id="8930d-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="8930d-111">Αυτό καθορίζει τον αριθμό των μηνυμάτων που μπορεί να στείλει ένας χρήστης από το λογαριασμό του Exchange Online μέσα σε μια καθορισμένη περίοδο.</span><span class="sxs-lookup"><span data-stu-id="8930d-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="8930d-112">Ο **μέγιστος αριθμός παραληπτών που επιτρέπονται στα πεδία "Προς", "Κοιν." και "Ιδιαίτ.** **1000 recipients**</span><span class="sxs-lookup"><span data-stu-id="8930d-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="8930d-113">Για να προσαρμόσετε αυτό το όριο, μεταβείτε [εδώ](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span><span class="sxs-lookup"><span data-stu-id="8930d-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
