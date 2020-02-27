---
title: Δημιουργήστε ένα email αλιευμάτων όλα
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 35f31c1662547d57c2fc9978ffb495ac29abcc01
ms.sourcegitcommit: 67015549afcbe05f3b77ea314e2ef7e0e439f9f2
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 02/26/2020
ms.locfileid: "42286193"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="eed1e-102">Δημιουργήστε ένα email αλιευμάτων όλα</span><span class="sxs-lookup"><span data-stu-id="eed1e-102">Create an email catch all</span></span>

<span data-ttu-id="eed1e-103">Η χρήση ενός αλιεύματος όλα αποθαρρύνεται έντονα.</span><span class="sxs-lookup"><span data-stu-id="eed1e-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="eed1e-104">Είναι καλύτερα να παρέχει μια αναπήδηση πίσω στον αποστολέα αφήνοντας τους αποστολείς γνωρίζουν το μήνυμά τους δεν θα μπορούσε να παραδοθεί ως απευθύνεται έτσι ώστε να μπορούν να αναλάβουν δράση.</span><span class="sxs-lookup"><span data-stu-id="eed1e-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="eed1e-105">Μπορείτε επίσης να περιορίσετε την εποπτευόμενη γραμματοκιβώτιο για να πιάσει μόνο πρώην έγκυρες διευθύνσεις ηλεκτρονικού ταχυδρομείου.</span><span class="sxs-lookup"><span data-stu-id="eed1e-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="eed1e-106">Κάθε αλιευμάτων όλα τα γραμματοκιβώτια θα λάβουν μια καλή συμφωνία των spam και μπορεί τελικά να συμπληρώσετε αν δεν παρακολουθούνται στενά.</span><span class="sxs-lookup"><span data-stu-id="eed1e-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="eed1e-107">(Υπάρχουν όρια παραλαβής.)</span><span class="sxs-lookup"><span data-stu-id="eed1e-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="eed1e-108">Εάν αποφασίσετε να συνεχίσετε, ακολουθήστε τα εξής βήματα:</span><span class="sxs-lookup"><span data-stu-id="eed1e-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="eed1e-109">Δημιουργήστε μια δυναμική ομάδα διανομής & συμπεριλάβετε "όλους τους τύπους παραληπτών."</span><span class="sxs-lookup"><span data-stu-id="eed1e-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="eed1e-110">Δημιουργήστε ένα αποκλειστικό γραμματοκιβώτιο για να πιάσει τα ηλεκτρονικά ταχυδρομεία, για παράδειγμα, catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="eed1e-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="eed1e-111">Για το συγκεκριμένο τομέα, ρυθμίστε το DomainType σε "InternalRelay".</span><span class="sxs-lookup"><span data-stu-id="eed1e-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="eed1e-112">Εάν αργότερα αφαιρέσετε τα αλιεύματα όλα, φροντίστε να ρυθμίσετε τον τομέα πίσω σε έγκυρες.</span><span class="sxs-lookup"><span data-stu-id="eed1e-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="eed1e-113">Δημιουργήστε έναν κανόνα μεταφοράς Mailflow ως εξής:</span><span class="sxs-lookup"><span data-stu-id="eed1e-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="eed1e-114">Εάν ο αποστολέας είναι "εκτός του οργανισμού"</span><span class="sxs-lookup"><span data-stu-id="eed1e-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="eed1e-115">Ανακατεύθυνση του μηνύματος σε Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="eed1e-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="eed1e-116">Εκτός αν ο παραλήπτης είναι μέλος της allusers@domain.com (ομάδα διανομής περιέχει όλα τα μέλη)</span><span class="sxs-lookup"><span data-stu-id="eed1e-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="eed1e-117">Βεβαιωθείτε για την επικύρωση ότι νέα γραμματοκιβώτια προστίθενται στη δυναμική ομάδα διανομής</span><span class="sxs-lookup"><span data-stu-id="eed1e-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
