---
title: Μετακίνηση μηνυμάτων ηλεκτρονικού ταχυδρομείου στο γραμματοκιβώτιο αρχειοθέτησης
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 9af8a4d3ce72fd901ff2f3a1aae0654c7213dd7e
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522771"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="14263-102">Μετακίνηση ηλεκτρονικού ταχυδρομείου στο γραμματοκιβώτιο αρχειοθέτησης</span><span class="sxs-lookup"><span data-stu-id="14263-102">Move email to the archive mailbox</span></span>

<span data-ttu-id="14263-103">Αν θέλετε να εκτελέσουμε αυτοματοποιημένους ελέγχους για τις ρυθμίσεις που αναφέρονται παρακάτω, επιλέξτε το κουμπί "Πίσω" <-- στο επάνω μέρος αυτής της σελίδας και, στη συνέχεια, πληκτρολογήστε τη διεύθυνση ηλεκτρονικού ταχυδρομείου του χρήστη που αντιμετωπίζει προβλήματα με τη μετακίνηση ηλεκτρονικού ταχυδρομείου στο γραμματοκιβώτιο αρχειοθέτησης.</span><span class="sxs-lookup"><span data-stu-id="14263-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems moving email to their archive mailbox.</span></span>

1. <span data-ttu-id="14263-104">Επιβεβαιώστε ότι έχει ενεργοποιηθεί ένα **γραμματοκιβώτιο αρχειοθέτησης.**</span><span class="sxs-lookup"><span data-stu-id="14263-104">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="14263-105">Εάν όχι, χρησιμοποιήστε τα βήματα [αυτού του άρθρου](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) για να ενεργοποιήσετε το γραμματοκιβώτιο αρχειοθέτησης.</span><span class="sxs-lookup"><span data-stu-id="14263-105">If not, use the steps in [this article](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="14263-106">Για να αρχειοθετηθούν αυτόματα τα μηνύματα στο γραμματοκιβώτιο αρχειοθέτησης, μια ετικέτα διατήρησης με την ενέργεια **Μετακίνηση στην αρχειοθέτηση** πρέπει να ρυθμιστεί ώστε να **εφαρμόζεται αυτόματα σε ολόκληρο το γραμματοκιβώτιο (προεπιλεγμένο) tag**.</span><span class="sxs-lookup"><span data-stu-id="14263-106">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="14263-107">Χρησιμοποιήστε τα βήματα εδώ για να δημιουργήσετε την ετικέτα: [Αρχειοθέτηση προεπιλεγμένη ετικέτα](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="14263-107">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="14263-108">Στη συνέχεια, προσθέστε την ετικέτα **Αρχειοθέτηση** στην πολιτική διατήρησης.</span><span class="sxs-lookup"><span data-stu-id="14263-108">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="14263-109">Στο κέντρο διαχείρισης του Exchange, επιλέξτε **Πολιτικές διατήρησης** > προσθέστε την **ετικέτα Μετακίνηση στην αρχειοθέτηση** στην πολιτική > **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="14263-109">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="14263-110">Τώρα [αντιστοιχίστε την πολιτική διατήρησης](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) στο γραμματοκιβώτιο του συγκεκριμένου χρήστη.</span><span class="sxs-lookup"><span data-stu-id="14263-110">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="14263-111">Η ίδια πολιτική θα εφαρμοστεί τόσο στο **γραμματοκιβώτιο "Κύρια"** όσο και στο γραμματοκιβώτιο **"Αρχειοθέτηση".**</span><span class="sxs-lookup"><span data-stu-id="14263-111">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="14263-112">Ίσως χρειαστεί να επιβάλετε την εκτέλεση και την εφαρμογή των νέων ρυθμίσεων από το Βοηθό διαχειριζόμενων φακέλων (MFA) και να εφαρμόσετε τις νέες ρυθμίσεις στο γραμματοκιβώτιο του χρήστη.</span><span class="sxs-lookup"><span data-stu-id="14263-112">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="14263-113">Εκτελέστε την ακόλουθη εντολή ενώ [είστε συνδεδεμένοι στο EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) για να ξεκινήσετε το Βοηθό διαχειριζόμενων φακέλων για ένα συγκεκριμένο γραμματοκιβώτιο:</span><span class="sxs-lookup"><span data-stu-id="14263-113">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="14263-114">Αρχή-Διαχειριζόμενη ΠτυχήAssistant -Ταυτότητα<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="14263-114">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="14263-115">Για περισσότερες πληροφορίες σχετικά με τη ρύθμιση μιας πολιτικής αρχειοθέτησης, ανατρέξτε στο θέμα [Ρύθμιση πολιτικής αρχειοθέτησης και διαγραφής για γραμματοκιβώτια](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="14263-115">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  