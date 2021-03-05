---
title: Μάθετε ποιος ρυθμίσει την προώθηση σε ένα γραμματοκιβώτιο και πώς
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50482298"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a><span data-ttu-id="f8fa2-102">Μάθετε ποιος ρυθμίσει την προώθηση σε ένα γραμματοκιβώτιο και πώς</span><span class="sxs-lookup"><span data-stu-id="f8fa2-102">Find out who set up forwarding on a mailbox, and how</span></span>

<span data-ttu-id="f8fa2-103">Εάν έχει οριστεί εξωτερική προώθηση σε ένα γραμματοκιβώτιο, η δραστηριότητα ελέγχονται ως μέρος του Set-Mailbox cmdlet.</span><span class="sxs-lookup"><span data-stu-id="f8fa2-103">If external forwarding was set on a mailbox, the activity is audited as part of the Set-Mailbox cmdlet.</span></span> <span data-ttu-id="f8fa2-104">Δείτε πώς μπορείτε να βρείτε τη δραστηριότητα στο αρχείο καταγραφής ελέγχου:</span><span class="sxs-lookup"><span data-stu-id="f8fa2-104">Here's how to find the activity in the audit log:</span></span>

1. <span data-ttu-id="f8fa2-105">Μεταβείτε στο [Κέντρο συμμόρφωσης ασφάλειας και συμμόρφωσης & του Office 365.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="f8fa2-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="f8fa2-106">Επιλέξτε **"Αναζήτηση** >  **αρχείου καταγραφής ελέγχου".**</span><span class="sxs-lookup"><span data-stu-id="f8fa2-106">Select **Search**> **Audit log search**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="f8fa2-107">Εάν δείτε μια ειδοποίηση ότι πρέπει να ενεργοποιήσετε τον έλεγχο, προχωρήστε και ενεργοποιήστε τον τώρα.</span><span class="sxs-lookup"><span data-stu-id="f8fa2-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="f8fa2-108">Εάν αυτή η δυνατότητα δεν είναι ενεργοποιημένη, τα αποτελέσματα αναζήτησης δεν θα είναι σε θέση να τραβήξει δεδομένα από προηγούμενες ημερομηνίες.</span><span class="sxs-lookup"><span data-stu-id="f8fa2-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="f8fa2-109">Βεβαιωθείτε ότι το πεδίο **"Δραστηριότητες"** έχει ρυθμιστεί **ώστε να εμφανίζει αποτελέσματα για όλες τις** δραστηριότητες (προεπιλογή).</span><span class="sxs-lookup"><span data-stu-id="f8fa2-109">Make sure the **Activities** field is set to **Show results for all activities** (the default).</span></span> <span data-ttu-id="f8fa2-110">Καθορίστε το εύρος ημερομηνιών.</span><span class="sxs-lookup"><span data-stu-id="f8fa2-110">Specify the date range.</span></span> <span data-ttu-id="f8fa2-111">Δεν χρειάζεται να καθορίσετε όνομα χρήστη.</span><span class="sxs-lookup"><span data-stu-id="f8fa2-111">You don't need to specify a username.</span></span>
1. <span data-ttu-id="f8fa2-112">Επιλέξτε **"Αναζήτηση".**</span><span class="sxs-lookup"><span data-stu-id="f8fa2-112">Select **Search**.</span></span> <span data-ttu-id="f8fa2-113">Οι δραστηριότητες εμφανίζονται στην περιοχή **"Αποτελέσματα".**</span><span class="sxs-lookup"><span data-stu-id="f8fa2-113">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="f8fa2-114">Επιλέξτε **"Αποτελέσματα φίλτρου"** και, στη **συνέχεια, πληκτρολογήστε "Ορισμός γραμματοκιβωτίου"** **στο πεδίο φίλτρου** "Δραστηριότητα".</span><span class="sxs-lookup"><span data-stu-id="f8fa2-114">Select **Filter Results**, and then enter **Set-mailbox** in the **Activity** filter field.</span></span> <span data-ttu-id="f8fa2-115">Αυτό επιστρέφει όλες τις **δραστηριότητες set-Mailbox.**</span><span class="sxs-lookup"><span data-stu-id="f8fa2-115">This returns all **Set-Mailbox** activities.</span></span>
1. <span data-ttu-id="f8fa2-116">Για να δείτε τις λεπτομέρειες, επιλέξτε μια δραστηριότητα και, στη συνέχεια, επιλέξτε **"Περισσότερες πληροφορίες".**</span><span class="sxs-lookup"><span data-stu-id="f8fa2-116">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="f8fa2-117">Στην περιοχή "Παράμετροι", μπορείτε να δείτε τη διεύθυνση ηλεκτρονικού ταχυδρομείου προώθησης που έχει οριστεί στο γραμματοκιβώτιο. </span><span class="sxs-lookup"><span data-stu-id="f8fa2-117">Under **Parameters** you can see the forwarding email address that was set on the mailbox.</span></span> <span data-ttu-id="f8fa2-118">Το **UserID** αντιπροσωπεύει το χρήστη που έχει ρυθμίσει την εξωτερική προώθηση στο γραμματοκιβώτιο.</span><span class="sxs-lookup"><span data-stu-id="f8fa2-118">The **UserID** represents the user who set up external forwarding on the mailbox.</span></span>
<span data-ttu-id="f8fa2-119">Για να μάθετε περισσότερα, ανατρέξτε στο [θέμα "Αναζήτηση στο αρχείο καταγραφής ελέγχου του Office 365" για να αντιμετωπίσετε συνηθισμένα σενάρια.](https://go.microsoft.com/fwlink/?linkid=2103944)</span><span class="sxs-lookup"><span data-stu-id="f8fa2-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>