---
title: Διαχείριση της καταχώρησης χρονικού
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004299"
- "7677"
ms.openlocfilehash: 2fcd0f386d2da8cad19fcc9872482bb75fe00dd2
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50745729"
---
# <a name="manage-journaling"></a><span data-ttu-id="201c5-102">Διαχείριση της καταχώρησης χρονικού</span><span class="sxs-lookup"><span data-stu-id="201c5-102">Manage journaling</span></span>

<span data-ttu-id="201c5-103">Η καταγραφή χρονικού μπορεί να βοηθήσει την εταιρεία σας να ανταποκριθεί στις νομικές, ρυθμιστικές και εταιρικές απαιτήσεις συμμόρφωσης, καταγράφοντας τις εισερχόμενες και εξερχόμενες επικοινωνίες ηλεκτρονικού ταχυδρομείου.</span><span class="sxs-lookup"><span data-stu-id="201c5-103">Journaling can help your organization respond to legal, regulatory, and organizational compliance requirements by recording inbound and outbound email communications.</span></span> <span data-ttu-id="201c5-104">Να έχετε υπόψη σας τα εξής:</span><span class="sxs-lookup"><span data-stu-id="201c5-104">Keep in mind:</span></span>

* <span data-ttu-id="201c5-105">Πρέπει να έχετε δικαιώματα [διαχείρισης οργανισμών](https://go.microsoft.com/fwlink/?linkid=2115259) και [διαχείρισης εγγραφών](https://go.microsoft.com/fwlink/?linkid=2115469) για να μπορείτε να διαχειριστείτε τη δημιουργία χρονικού.</span><span class="sxs-lookup"><span data-stu-id="201c5-105">You need to have [Organization Management](https://go.microsoft.com/fwlink/?linkid=2115259) and [Records Management](https://go.microsoft.com/fwlink/?linkid=2115469) permissions before you can manage journaling.</span></span>
* <span data-ttu-id="201c5-106">Πρέπει να έχετε ένα γραμματοκιβώτιο χρονικού και (προαιρετικά) να ρυθμίσετε τις παραμέτρους ενός εναλλακτικού γραμματοκιβωτίου χρονικού.</span><span class="sxs-lookup"><span data-stu-id="201c5-106">You need to have a journal mailbox and (optionally) an alternate journaling mailbox configured.</span></span> <span data-ttu-id="201c5-107">Για να μάθετε περισσότερα, ανατρέξτε στο [θέμα Ρύθμιση παραμέτρων χρονικού στο Exchange Online.](https://go.microsoft.com/fwlink/?linkid=2115260)</span><span class="sxs-lookup"><span data-stu-id="201c5-107">To learn more, see [Configure Journaling in Exchange Online](https://go.microsoft.com/fwlink/?linkid=2115260).</span></span>
* <span data-ttu-id="201c5-108">Στο Exchange Online, υπάρχει όριο στον αριθμό των κανόνων χρονικού που μπορείτε να δημιουργήσετε.</span><span class="sxs-lookup"><span data-stu-id="201c5-108">In Exchange Online, there's a limit to the number of journal rules that you can create.</span></span> <span data-ttu-id="201c5-109">Για λεπτομέρειες, ανατρέξτε [στο θέμα "Χρονικό", "Μεταφορά" και "Όρια κανόνων εισερχομένων".](https://go.microsoft.com/fwlink/?linkid=2115261)</span><span class="sxs-lookup"><span data-stu-id="201c5-109">For details, see [Journal, transport, and inbox rule limits](https://go.microsoft.com/fwlink/?linkid=2115261).</span></span>
* <span data-ttu-id="201c5-110">Το Exchange Online δεν υποστηρίζει την παράδοση αναφορών χρονικού σε γραμματοκιβώτιο του Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="201c5-110">Exchange Online doesn't support delivering journal reports to an Exchange Online mailbox.</span></span> <span data-ttu-id="201c5-111">Πρέπει να καθορίσετε τη διεύθυνση ηλεκτρονικού ταχυδρομείου ενός συστήματος αρχειοθέτησης εσωτερικής εγκατάστασης ή μιας υπηρεσίας αρχειοθέτησης άλλου κατασκευαστή ως γραμματοκιβωτίου καταχώρησης χρονικού.</span><span class="sxs-lookup"><span data-stu-id="201c5-111">You must specify the email address of an on-premises archiving system or a third-party archiving service as the journaling mailbox.</span></span>
