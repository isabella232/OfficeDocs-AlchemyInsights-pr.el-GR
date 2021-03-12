---
title: Αυτόματη μετακίνηση μηνυμάτων ηλεκτρονικού ταχυδρομείου στο γραμματοκιβώτιο αρχειοθέτησης
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746041"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a><span data-ttu-id="cd845-102">Αυτόματη μετακίνηση μηνυμάτων ηλεκτρονικού ταχυδρομείου στο γραμματοκιβώτιο αρχειοθέτησης</span><span class="sxs-lookup"><span data-stu-id="cd845-102">Automatically move email messages to the archive mailbox</span></span>

<span data-ttu-id="cd845-103">Δείτε πώς μπορείτε να ρυθμίσετε μια πολιτική για την αυτόματη μετακίνηση του παλιού ηλεκτρονικού ταχυδρομείου ενός χρήστη στο γραμματοκιβώτιο αρχειοθέτησης:</span><span class="sxs-lookup"><span data-stu-id="cd845-103">Here's how to set up a policy to automatically move a user's old email to the archive mailbox:</span></span>

1. <span data-ttu-id="cd845-104">Μεταβείτε [**στην "& Αρχειοθέτηση διαχείρισης**](https://go.microsoft.com/fwlink/p/?linkid=2077143)δεδομένων  >  **συμμόρφωσης"** για να  >   επαληθεύσετε ότι έχει ενεργοποιηθεί ένα γραμματοκιβώτιο αρχειοθέτησης για το χρήστη.</span><span class="sxs-lookup"><span data-stu-id="cd845-104">Go to [**Security & Compliance**](https://go.microsoft.com/fwlink/p/?linkid=2077143) > **Data governance** > **Archive** to verify an archive mailbox has been enabled for the user.</span></span> <span data-ttu-id="cd845-105">Εάν δεν το έχει κάνει, κάντε κλικ στην επιλογή **"Ενεργοποίηση"** **και, στη συνέχεια, "Ναι"** στο πλαίσιο προειδοποίησης.</span><span class="sxs-lookup"><span data-stu-id="cd845-105">If it hasn't, click **Enable** then **Yes** in the warning box.</span></span>
2. <span data-ttu-id="cd845-106">Μεταβείτε [**στο Κέντρο διαχείρισης του Exchange > διαχείριση συμμόρφωσης > ετικέτες διατήρησης.**](https://go.microsoft.com/fwlink/?linkid=2059104)</span><span class="sxs-lookup"><span data-stu-id="cd845-106">Go to [**Exchange admin center > compliance management > retention tags**](https://go.microsoft.com/fwlink/?linkid=2059104).</span></span>
3. <span data-ttu-id="cd845-107">Επιλέξτε το εικονίδιο + και, στη **συνέχεια, επιλέξτε αυτόματη εφαρμογή σε ολόκληρο το γραμματοκιβώτιο.**</span><span class="sxs-lookup"><span data-stu-id="cd845-107">Choose the + icon then choose **automatically apply to entire mailbox**.</span></span>
4. <span data-ttu-id="cd845-108">Αντιστοιχίστε ένα όνομα στην ετικέτα διατήρησης και επιλέξτε **"Μετακίνηση στην Αρχειοθήκη".**</span><span class="sxs-lookup"><span data-stu-id="cd845-108">Assign a name to the retention tag, and choose **Move to Archive**.</span></span> <span data-ttu-id="cd845-109">Για την περίοδο διατήρησης, εισαγάγετε το χρόνο που θέλετε, όπως 90 ημέρες.</span><span class="sxs-lookup"><span data-stu-id="cd845-109">For the retention period, enter the time you want, such as 90 days.</span></span> <span data-ttu-id="cd845-110">Επιλέξτε **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="cd845-110">Click **Save**.</span></span>
5. <span data-ttu-id="cd845-111">Τώρα δημιουργήστε μια πολιτική διατήρησης: επιλέξτε **πολιτικές διατήρησης,** επιλέξτε το εικονίδιο για να προσθέσετε μια νέα πολιτική.</span><span class="sxs-lookup"><span data-stu-id="cd845-111">Now create a retention policy: choose **retention policies**, choose the icon to add a new policy.</span></span>
6. <span data-ttu-id="cd845-112">Αντιστοιχίστε ένα όνομα στην πολιτική διατήρησης και, στη συνέχεια, κάντε κλικ και κάντε κύλιση για να βρείτε και να προσθέσετε την ετικέτα διατήρησης που μόλις δημιουργήσατε.</span><span class="sxs-lookup"><span data-stu-id="cd845-112">Assign a name to the retention policy, then click and scroll to find and add the retention tag you just created.</span></span> <span data-ttu-id="cd845-113">Επιλέξτε **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="cd845-113">Click **Save**.</span></span>
7. <span data-ttu-id="cd845-114">Τέλος, εφαρμόστε την πολιτική διατήρησης στο γραμματοκιβώτιο του χρήστη: εξακολουθείτε να είστε στο κέντρο διαχείρισης του Exchange, μεταβείτε **στα γραμματοκιβώτια**  >  **παραληπτών.**</span><span class="sxs-lookup"><span data-stu-id="cd845-114">Finally, apply the retention policy to the user's mailbox: still in the Exchange admin center, go to **recipients** > **mailboxes**.</span></span> <span data-ttu-id="cd845-115">Επιλέξτε όλους τους χρήστες στους οποίοι θέλετε να εφαρμόσετε την πολιτική και, στη συνέχεια, επιλέξτε **"Επεξεργασία"** (το εικονίδιο μολυβιού).</span><span class="sxs-lookup"><span data-stu-id="cd845-115">Choose all the users who you want to apply the policy to, then choose **Edit** (the pencil icon).</span></span>
8. <span data-ttu-id="cd845-116">Στο παράθυρο διαλόγου, κάντε κλικ στις δυνατότητες **γραμματοκιβωτίου.**</span><span class="sxs-lookup"><span data-stu-id="cd845-116">In the dialog box, click **mailbox features**.</span></span> <span data-ttu-id="cd845-117">Στην **περιοχή "Πολιτική** διατήρησης", εφαρμόστε την πολιτική που μόλις δημιουργήσατε > **Αποθήκευση.**</span><span class="sxs-lookup"><span data-stu-id="cd845-117">Under **Retention policy**, apply the policy you just created > **Save**.</span></span>
9. <span data-ttu-id="cd845-118">Για οδηγίες σχετικά με την εφαρμογή της πολιτικής σε όλους τους χρήστες, ανατρέξτε στο θέμα [Εφαρμογή πολιτικής διατήρησης σε γραμματοκιβώτια.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)</span><span class="sxs-lookup"><span data-stu-id="cd845-118">For instructions for applying the policy to all users, see [Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).</span></span>
