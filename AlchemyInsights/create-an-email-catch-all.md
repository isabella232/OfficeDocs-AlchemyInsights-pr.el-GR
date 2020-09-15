---
title: Δημιουργία μηνύματος ηλεκτρονικού ταχυδρομείου "catch all"
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 262d2c6a7181d94094f3d840c4ba3ebd07000cf4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712986"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="421be-102">Δημιουργία μηνύματος ηλεκτρονικού ταχυδρομείου "catch all"</span><span class="sxs-lookup"><span data-stu-id="421be-102">Create an email catch all</span></span>

<span data-ttu-id="421be-103">Η χρήση των αλιευμάτων δεν αποθαρρύνεται ιδιαίτερα.</span><span class="sxs-lookup"><span data-stu-id="421be-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="421be-104">Είναι προτιμότερο να παρέχετε μια αναπήδηση πίσω στον αποστολέα, αφήνοντας τους αποστολείς να γνωρίζουν ότι το μήνυμά τους δεν μπορεί να παραδοθεί με τον τρόπο που απευθύνεται, ώστε να μπορούν να αναλάβουν δράση.</span><span class="sxs-lookup"><span data-stu-id="421be-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="421be-105">Μπορείτε επίσης να περιορίσετε το γραμματοκιβώτιο που παρακολουθείται για τη σύλληψη μόνο των πρώην έγκυρων διευθύνσεων ηλεκτρονικού ταχυδρομείου.</span><span class="sxs-lookup"><span data-stu-id="421be-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="421be-106">Οποιαδήποτε αλιεύματα όλα τα γραμματοκιβώτια θα λαμβάνουν πολύ ανεπιθύμητη αλληλογραφία και μπορεί τελικά να συμπληρωθούν εάν δεν παρακολουθούνται στενά.</span><span class="sxs-lookup"><span data-stu-id="421be-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="421be-107">(Υπάρχουν όρια παραλαβής.)</span><span class="sxs-lookup"><span data-stu-id="421be-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="421be-108">Εάν αποφασίσετε να συνεχίσετε, ακολουθήστε τα παρακάτω βήματα:</span><span class="sxs-lookup"><span data-stu-id="421be-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="421be-109">Δημιουργήστε μια δυναμική ομάδα διανομής & συμπεριλάβετε "όλους τους τύπους παραληπτών".</span><span class="sxs-lookup"><span data-stu-id="421be-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="421be-110">Δημιουργήστε ένα αποκλειστικό γραμματοκιβώτιο για να πιάνετε μηνύματα ηλεκτρονικού ταχυδρομείου, για παράδειγμα, catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="421be-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="421be-111">Για τον συγκεκριμένο τομέα, ορίστε το DomainType σε "InternalRelay".</span><span class="sxs-lookup"><span data-stu-id="421be-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="421be-112">Εάν αργότερα καταργήσετε όλα τα αλιεύματα, βεβαιωθείτε ότι έχετε ρυθμίσει τον τομέα ξανά σε επιτακτική.</span><span class="sxs-lookup"><span data-stu-id="421be-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="421be-113">Δημιουργήστε έναν κανόνα μεταφοράς Mailflow ως εξής:</span><span class="sxs-lookup"><span data-stu-id="421be-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="421be-114">Εάν ο αποστολέας είναι "εκτός του οργανισμού"</span><span class="sxs-lookup"><span data-stu-id="421be-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="421be-115">Ανακατεύθυνση του μηνύματος στο Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="421be-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="421be-116">Εκτός εάν ο παραλήπτης είναι μέλος του allusers@domain.com (η ομάδα διανομής περιέχει όλα τα μέλη)</span><span class="sxs-lookup"><span data-stu-id="421be-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="421be-117">Βεβαιωθείτε ότι έχετε προσθέσει νέα γραμματοκιβώτια στη δυναμική ομάδα διανομής</span><span class="sxs-lookup"><span data-stu-id="421be-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
