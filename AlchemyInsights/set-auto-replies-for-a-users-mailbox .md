---
title: Ορισμός αυτόματων απαντήσεων για το γραμματοκιβώτιο ενός χρήστη
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: e3cc01298c10fd3ba21327a7fb5cc5396d0ad74d
ms.sourcegitcommit: 23e5b94f1758bfe202008384e300b81816975375
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43506518"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a><span data-ttu-id="7e850-102">Ορισμός αυτόματων απαντήσεων για το γραμματοκιβώτιο ενός χρήστη</span><span class="sxs-lookup"><span data-stu-id="7e850-102">Set auto replies for a user's mailbox</span></span>

<span data-ttu-id="7e850-103">**Μέθοδος 1**</span><span class="sxs-lookup"><span data-stu-id="7e850-103">**Method 1**</span></span>

1. <span data-ttu-id="7e850-104">Είσοδος στην πύλη του Office 365.</span><span class="sxs-lookup"><span data-stu-id="7e850-104">Sign in to the Office 365 portal.</span></span>

2. <span data-ttu-id="7e850-105">Μεταβείτε στην επιλογή **Χρήστες > Ενεργοί χρήστες** (ή **Ομάδες > Κοινόχρηστα γραμματοκιβώτια** εάν έχετε κάνει αυτή τη ρύθμιση σε ένα κοινόχρηστο γραμματοκιβώτιο).</span><span class="sxs-lookup"><span data-stu-id="7e850-105">Go to **Users > Active users** (or **Groups > Shared mailboxes** if you set this on a shared mailbox).</span></span>

3. <span data-ttu-id="7e850-106">Επιλέξτε έναν χρήστη που έχει γραμματοκιβώτιο του Microsoft Exchange.</span><span class="sxs-lookup"><span data-stu-id="7e850-106">Select a user who has a Microsoft Exchange mailbox.</span></span>

4. <span data-ttu-id="7e850-107">Στο αναδυόμενο μενού στα δεξιά, μεταβείτε στις **Ρυθμίσεις αλληλογραφίας > Αυτόματες απαντήσεις** (εάν πρόκειται για ένα κοινόχρηστο γραμματοκιβώτιο, απλώς κάντε κλικ στην επιλογή **Αυτόματες απαντήσεις** στο αναδυόμενο μενού).</span><span class="sxs-lookup"><span data-stu-id="7e850-107">On the fly-out menu on the right, go to **Mail settings > Automatic replies** (if it's a shared mailbox, just click **Automatic replies** on the fly-out).</span></span>

<span data-ttu-id="7e850-108">**Μέθοδος 2**</span><span class="sxs-lookup"><span data-stu-id="7e850-108">**Method 2**</span></span>

1. <span data-ttu-id="7e850-109">Πραγματοποιήστε είσοδο στην πύλη διαχείρισης του Office 365, χρησιμοποιώντας τα διαπιστευτήρια διαχειριστή.</span><span class="sxs-lookup"><span data-stu-id="7e850-109">Sign in to the Office 365 admin portal by using administrator credentials.</span></span>

2. <span data-ttu-id="7e850-110">Αναπτύξτε τα **Κέντρα διαχείρισης** και, στη συνέχεια, κάντε κλικ στην επιλογή **Ανταλλαγή**.</span><span class="sxs-lookup"><span data-stu-id="7e850-110">Expand **Admin Centers**, and then click **Exchange**.</span></span>

3. <span data-ttu-id="7e850-111">Κάντε κλικ στην εικόνα στην επάνω δεξιά γωνία, κάντε κλικ στην επιλογή **Άλλος χρήστης** και, στη συνέχεια, επιλέξτε το γραμματοκιβώτιο χρήστη που θέλετε να αλλάξετε.</span><span class="sxs-lookup"><span data-stu-id="7e850-111">Click the picture in the upper-right corner, click **Another User**, and then select the user mailbox that you want to change.</span></span>

4. <span data-ttu-id="7e850-112">Στην αριστερή πλευρά, επιλέξτε **Επιλογές**, κάντε κλικ στην επιλογή **Οργάνωση ηλεκτρονικού ταχυδρομείου** και, στη συνέχεια, κάντε κλικ στην επιλογή **Αυτόματες απαντήσεις.**</span><span class="sxs-lookup"><span data-stu-id="7e850-112">On the left side, select **Options**, click **Organize E-mail**, and then click **Automatic replies.**</span></span>

<span data-ttu-id="7e850-113">**Μέθοδος 3**</span><span class="sxs-lookup"><span data-stu-id="7e850-113">**Method 3**</span></span>

<span data-ttu-id="7e850-114">Εκτελέστε το ακόλουθο cmdlet στο Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="7e850-114">Run the following cmdlet in Exchange Online PowerShell:</span></span>

<span data-ttu-id="7e850-115">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="7e850-115">PowerShellCopy</span></span>

    Set-MailboxAutoReplyConfiguration

<span data-ttu-id="7e850-116">Για περισσότερες πληροφορίες σχετικά με αυτό το cmdlet, ανατρέξτε στο θέμα [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span><span class="sxs-lookup"><span data-stu-id="7e850-116">For more information about this cmdlet, see [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span></span>
