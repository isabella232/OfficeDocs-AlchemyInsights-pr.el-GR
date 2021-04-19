---
title: Χρειάζεστε βοήθεια σχετικά με τα όρια αποστολής μηνυμάτων ηλεκτρονικού ταχυδρομείου;
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
- "9002938"
- "5630"
ms.openlocfilehash: b5bdfbf818328c97ec93b3468aeedcbe88e03913
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836279"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="52ecc-102">Χρειάζεστε βοήθεια σχετικά με τα όρια αποστολής μηνυμάτων ηλεκτρονικού ταχυδρομείου;</span><span class="sxs-lookup"><span data-stu-id="52ecc-102">Need help with email sending limits?</span></span>

<span data-ttu-id="52ecc-103">Ακολουθούν τα όρια **αποστολής μέσω σχεδίου που** επιβάλλονται στην υπηρεσία.</span><span class="sxs-lookup"><span data-stu-id="52ecc-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="52ecc-104">Περισσότερες πληροφορίες σχετικά με αυτά τα όρια τεκμηριώνονται [εδώ.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits)</span><span class="sxs-lookup"><span data-stu-id="52ecc-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="52ecc-105">Για να αποθαρρύνουμε την παράδοση αυτόκλητων μαζικών μηνυμάτων, εφαρμόζονται όρια χρέωσης παραλήπτη ανά χρήστη **σε όλα τα εξερχόμενα και εσωτερικά μηνύματα.**</span><span class="sxs-lookup"><span data-stu-id="52ecc-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="52ecc-106">Σε όλες τις SKUs, αυτό το όριο **είναι 10.000 παραλήπτες ανά ημέρα.**</span><span class="sxs-lookup"><span data-stu-id="52ecc-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="52ecc-107">Οι πελάτες που πρέπει να στείλουν νόμιμα μαζικά εμπορικά μηνύματα ηλεκτρονικού ταχυδρομείου (για παράδειγμα, ενημερωτικά δελτία πελατών) θα πρέπει να χρησιμοποιούν υπηρεσίες παροχής τρίτων που ειδικεύονται σε αυτές τις υπηρεσίες.</span><span class="sxs-lookup"><span data-stu-id="52ecc-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="52ecc-108">**Σημείωση:** Όταν επιτευχθεί το όριο χρέωσης του παραλήπτη, τα μηνύματα δεν μπορούν να αποσταλούν από το γραμματοκιβώτιο μέχρι ο αριθμός των παραληπτών που στάλθηκαν τα μηνύματα τις τελευταίες 24 ώρες να πέσει κάτω από το όριο.</span><span class="sxs-lookup"><span data-stu-id="52ecc-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="52ecc-109">Ο χρήστης δεν θα μπορεί να στείλει μηνύματα μέχρι αυτό το σημείο.</span><span class="sxs-lookup"><span data-stu-id="52ecc-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="52ecc-110">Το όριο χρέωσης μηνυμάτων **των 30 μηνυμάτων ανά λεπτό** εφαρμόζεται σε όλες τις SKUs.</span><span class="sxs-lookup"><span data-stu-id="52ecc-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="52ecc-111">Αυτό καθορίζει πόσα μηνύματα μπορεί να στείλει ένας χρήστης από το λογαριασμό του Exchange Online μέσα σε μια καθορισμένη περίοδο.</span><span class="sxs-lookup"><span data-stu-id="52ecc-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="52ecc-112">Ο **μέγιστος αριθμός παραληπτών** που επιτρέπονται στα πεδία "Προς", "Κοιν." και "Κοιν." για ένα μεμονωμένο μήνυμα ηλεκτρονικού ταχυδρομείου, σε όλες τις SKUs, είναι **1.000 παραλήπτες.**</span><span class="sxs-lookup"><span data-stu-id="52ecc-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="52ecc-113">Για να προσαρμόσετε αυτό το όριο, [μεταβείτε εδώ.](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228)</span><span class="sxs-lookup"><span data-stu-id="52ecc-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
