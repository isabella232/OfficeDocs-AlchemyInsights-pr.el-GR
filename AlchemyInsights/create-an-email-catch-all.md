---
title: Δημιουργήστε ένα μήνυμα ηλεκτρονικού ταχυδρομείου για να τα πιάσετε όλα
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 2b9131a620139a93ddb844fd49d8fa2ed68e52c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816200"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="27d77-102">Δημιουργήστε ένα μήνυμα ηλεκτρονικού ταχυδρομείου για να τα πιάσετε όλα</span><span class="sxs-lookup"><span data-stu-id="27d77-102">Create an email catch all</span></span>

<span data-ttu-id="27d77-103">Η χρήση ενός catch all είναι έντονα αποθαρρυνθεί.</span><span class="sxs-lookup"><span data-stu-id="27d77-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="27d77-104">Είναι καλύτερα να παρέχετε μια αναπήδηση στον αποστολέα που να επιτρέπει στους αποστολείς να γνωρίζουν ότι το μήνυμά τους δεν ήταν δυνατό να παραδοθεί ως απευθύνεται, ώστε να μπορούν να κάνουν ενέργειες.</span><span class="sxs-lookup"><span data-stu-id="27d77-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="27d77-105">Μπορείτε επίσης να περιορίσετε το γραμματοκιβώτιο που παρακολουθείται ώστε να περιλαμβάνει μόνο παλαιότερες έγκυρες διευθύνσεις ηλεκτρονικού ταχυδρομείου.</span><span class="sxs-lookup"><span data-stu-id="27d77-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="27d77-106">Κάθε λήψη όλων των γραμματοκιβωτίων θα λαμβάνει πολλές ανεπιθύμητη αλληλογραφία και μπορεί τελικά να γεμίσει, εάν δεν παρακολουθείται στενά.</span><span class="sxs-lookup"><span data-stu-id="27d77-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="27d77-107">(Υπάρχουν όρια λήψης.)</span><span class="sxs-lookup"><span data-stu-id="27d77-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="27d77-108">Εάν αποφασίσετε να προχωρήσετε, ακολουθήστε τα παρακάτω βήματα:</span><span class="sxs-lookup"><span data-stu-id="27d77-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="27d77-109">Δημιουργήστε μια δυναμική ομάδα διανομής και & "Όλοι οι τύποι παραληπτών".</span><span class="sxs-lookup"><span data-stu-id="27d77-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="27d77-110">Δημιουργήστε ένα αποκλειστικό γραμματοκιβώτιο για να λαμβάνετε μηνύματα ηλεκτρονικού ταχυδρομείου, για παράδειγμα, catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="27d77-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="27d77-111">Για τον συγκεκριμένο τομέα, ορίστε το DomainType σε "InternalRelay".</span><span class="sxs-lookup"><span data-stu-id="27d77-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="27d77-112">Εάν αργότερα καταργήσετε το catch all, φροντίστε να ορίσετε ξανά τον τομέα σε "Έγκυρα".</span><span class="sxs-lookup"><span data-stu-id="27d77-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="27d77-113">Δημιουργήστε έναν κανόνα μεταφοράς ροής αλληλογραφίας ως εξής:</span><span class="sxs-lookup"><span data-stu-id="27d77-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="27d77-114">Εάν ο αποστολέας είναι "Εκτός του οργανισμού"</span><span class="sxs-lookup"><span data-stu-id="27d77-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="27d77-115">Ανακατεύθυνση του μηνύματος σε Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="27d77-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="27d77-116">Εκτός εάν ο παραλήπτης είναι μέλος του allusers@domain.com (Η ομάδα διανομής περιέχει όλα τα μέλη)</span><span class="sxs-lookup"><span data-stu-id="27d77-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="27d77-117">Βεβαιωθείτε ότι έχουν προστεθεί νέα γραμματοκιβώτια στη Δυναμική ομάδα διανομής</span><span class="sxs-lookup"><span data-stu-id="27d77-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
