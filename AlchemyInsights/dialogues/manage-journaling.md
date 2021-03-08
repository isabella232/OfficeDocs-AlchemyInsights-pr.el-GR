---
title: Διαχείριση καταχώρησης σε χρονικό
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
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524632"
---
# <a name="manage-journaling"></a><span data-ttu-id="740c4-102">Διαχείριση καταχώρησης σε χρονικό</span><span class="sxs-lookup"><span data-stu-id="740c4-102">Manage journaling</span></span>

<span data-ttu-id="740c4-103">Η καταχώρηση σε χρονικό μπορεί να βοηθήσει τον οργανισμό σας να ανταποκριθεί στις νομικές απαιτήσεις, τις ρυθμιστικές απαιτήσεις και τις απαιτήσεις εταιρικής συμμόρφωσης, καταγράφοντας τις επικοινωνίες εισερχομένων και εξερχόμενων μηνυμάτων ηλεκτρονικού ταχυδρομείου.</span><span class="sxs-lookup"><span data-stu-id="740c4-103">Journaling can help your organization respond to legal, regulatory, and organizational compliance requirements by recording inbound and outbound email communications.</span></span> <span data-ttu-id="740c4-104">Να έχετε υπόψη τα εξής:</span><span class="sxs-lookup"><span data-stu-id="740c4-104">Keep in mind:</span></span>

* <span data-ttu-id="740c4-105">Πρέπει να έχετε δικαιώματα [Διαχείρισης διαχείρισης και](https://go.microsoft.com/fwlink/?linkid=2115259) διαχείρισης εγγραφών οργανισμού [για](https://go.microsoft.com/fwlink/?linkid=2115469) να διαχειριστείτε την καταχώρηση σε χρονικό.</span><span class="sxs-lookup"><span data-stu-id="740c4-105">You need to have [Organization Management](https://go.microsoft.com/fwlink/?linkid=2115259) and [Records Management](https://go.microsoft.com/fwlink/?linkid=2115469) permissions before you can manage journaling.</span></span>
* <span data-ttu-id="740c4-106">Πρέπει να έχετε ένα γραμματοκιβώτιο χρονικού και (προαιρετικά) να ρυθμίσετε τις παραμέτρους ενός εναλλακτικού γραμματοκιβωτίου καταχώρησης σε χρονικό.</span><span class="sxs-lookup"><span data-stu-id="740c4-106">You need to have a journal mailbox and (optionally) an alternate journaling mailbox configured.</span></span> <span data-ttu-id="740c4-107">Για να μάθετε περισσότερα, ανατρέξτε στο [θέμα "Ρύθμιση παραμέτρων καταχώρησης σε χρονικό" στο Exchange Online.](https://go.microsoft.com/fwlink/?linkid=2115260)</span><span class="sxs-lookup"><span data-stu-id="740c4-107">To learn more, see [Configure Journaling in Exchange Online](https://go.microsoft.com/fwlink/?linkid=2115260).</span></span>
* <span data-ttu-id="740c4-108">Στο Exchange Online, υπάρχει ένα όριο στον αριθμό των κανόνων χρονικού που μπορείτε να δημιουργήσετε.</span><span class="sxs-lookup"><span data-stu-id="740c4-108">In Exchange Online, there's a limit to the number of journal rules that you can create.</span></span> <span data-ttu-id="740c4-109">Για λεπτομέρειες, ανατρέξτε [στα όρια χρονικού, μεταφοράς και κανόνων εισερχομένων.](https://go.microsoft.com/fwlink/?linkid=2115261)</span><span class="sxs-lookup"><span data-stu-id="740c4-109">For details, see [Journal, transport, and inbox rule limits](https://go.microsoft.com/fwlink/?linkid=2115261).</span></span>
* <span data-ttu-id="740c4-110">Το Exchange Online δεν υποστηρίζει την παράδοση αναφορών χρονικού σε ένα γραμματοκιβώτιο του Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="740c4-110">Exchange Online doesn't support delivering journal reports to an Exchange Online mailbox.</span></span> <span data-ttu-id="740c4-111">Πρέπει να καθορίσετε τη διεύθυνση ηλεκτρονικού ταχυδρομείου ενός συστήματος αρχειοθέτησης εσωτερικής εγκατάστασης ή μιας υπηρεσίας αρχειοθέτησης τρίτου κατασκευαστή ως γραμματοκιβώτιο καταχώρησης σε χρονικό.</span><span class="sxs-lookup"><span data-stu-id="740c4-111">You must specify the email address of an on-premises archiving system or a third-party archiving service as the journaling mailbox.</span></span>
