---
title: Ορισμός αυτόματων απαντήσεων για ένα γραμματοκιβώτιο
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
- "9000761"
- "3514"
ms.openlocfilehash: 60af581e7fe508ab9644a53873bcd551b3aacff1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820934"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a><span data-ttu-id="25c3c-102">Ορισμός αυτόματων απαντήσεων για το γραμματοκιβώτιο ενός χρήστη</span><span class="sxs-lookup"><span data-stu-id="25c3c-102">Set auto replies for a user's mailbox</span></span>

<span data-ttu-id="25c3c-103">**Μέθοδος 1**</span><span class="sxs-lookup"><span data-stu-id="25c3c-103">**Method 1**</span></span>

1. <span data-ttu-id="25c3c-104">Είσοδος στην πύλη Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="25c3c-104">Sign in to the Microsoft 365 portal.</span></span>

2. <span data-ttu-id="25c3c-105">Μεταβείτε στην επιλογή **Χρήστες > Ενεργοί χρήστες** (ή **Ομάδες > Κοινόχρηστα γραμματοκιβώτια** εάν έχετε κάνει αυτή τη ρύθμιση σε ένα κοινόχρηστο γραμματοκιβώτιο).</span><span class="sxs-lookup"><span data-stu-id="25c3c-105">Go to **Users > Active users** (or **Groups > Shared mailboxes** if you set this on a shared mailbox).</span></span>

3. <span data-ttu-id="25c3c-106">Επιλέξτε έναν χρήστη που έχει γραμματοκιβώτιο του Microsoft Exchange.</span><span class="sxs-lookup"><span data-stu-id="25c3c-106">Select a user who has a Microsoft Exchange mailbox.</span></span>

4. <span data-ttu-id="25c3c-107">Στο αναδυόμενο μενού στα δεξιά, μεταβείτε στις **Ρυθμίσεις αλληλογραφίας > Αυτόματες απαντήσεις** (εάν πρόκειται για ένα κοινόχρηστο γραμματοκιβώτιο, απλώς κάντε κλικ στην επιλογή **Αυτόματες απαντήσεις** στο αναδυόμενο μενού).</span><span class="sxs-lookup"><span data-stu-id="25c3c-107">On the fly-out menu on the right, go to **Mail settings > Automatic replies** (if it's a shared mailbox, just click **Automatic replies** on the fly-out).</span></span>

<span data-ttu-id="25c3c-108">**Μέθοδος 2**</span><span class="sxs-lookup"><span data-stu-id="25c3c-108">**Method 2**</span></span>

1. <span data-ttu-id="25c3c-109">Πραγματοποιήστε είσοδο στην πύλη διαχείρισης του Microsoft 365, χρησιμοποιώντας τα διαπιστευτήρια διαχειριστή.</span><span class="sxs-lookup"><span data-stu-id="25c3c-109">Sign in to the Microsoft 365 admin portal by using administrator credentials.</span></span>

2. <span data-ttu-id="25c3c-110">Αναπτύξτε τα **Κέντρα διαχείρισης** και, στη συνέχεια, κάντε κλικ στην επιλογή **Ανταλλαγή**.</span><span class="sxs-lookup"><span data-stu-id="25c3c-110">Expand **Admin Centers**, and then click **Exchange**.</span></span>

3. <span data-ttu-id="25c3c-111">Κάντε κλικ στην εικόνα στην επάνω δεξιά γωνία, κάντε κλικ στην επιλογή **Άλλος χρήστης** και, στη συνέχεια, επιλέξτε το γραμματοκιβώτιο χρήστη που θέλετε να αλλάξετε.</span><span class="sxs-lookup"><span data-stu-id="25c3c-111">Click the picture in the upper-right corner, click **Another User**, and then select the user mailbox that you want to change.</span></span>

4. <span data-ttu-id="25c3c-112">Στην αριστερή πλευρά, επιλέξτε **Επιλογές**, κάντε κλικ στην επιλογή **Οργάνωση ηλεκτρονικού ταχυδρομείου** και, στη συνέχεια, κάντε κλικ στην επιλογή **Αυτόματες απαντήσεις.**</span><span class="sxs-lookup"><span data-stu-id="25c3c-112">On the left side, select **Options**, click **Organize E-mail**, and then click **Automatic replies.**</span></span>

<span data-ttu-id="25c3c-113">**Μέθοδος 3**</span><span class="sxs-lookup"><span data-stu-id="25c3c-113">**Method 3**</span></span>

<span data-ttu-id="25c3c-114">Εκτελέστε το ακόλουθο cmdlet στο Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="25c3c-114">Run the following cmdlet in Exchange Online PowerShell:</span></span>

<span data-ttu-id="25c3c-115">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="25c3c-115">PowerShellCopy</span></span>

```
    Set-MailboxAutoReplyConfiguration
```

<span data-ttu-id="25c3c-116">Για περισσότερες πληροφορίες σχετικά με αυτό το cmdlet, ανατρέξτε στο θέμα [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span><span class="sxs-lookup"><span data-stu-id="25c3c-116">For more information about this cmdlet, see [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span></span>
