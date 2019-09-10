---
title: Μετακίνηση μηνυμάτων ηλεκτρονικού ταχυδρομείου στο γραμματοκιβώτιο αρχειοθέτησης
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 5592bc7d4566e3498c33bbf9488db7f46ec58842
ms.sourcegitcommit: 8864b5789d9905916039081b53530c7e6d8bc529
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822162"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="10536-102">Μετακίνηση ηλεκτρονικού ταχυδρομείου στο γραμματοκιβώτιο αρχειοθέτησης</span><span class="sxs-lookup"><span data-stu-id="10536-102">Move email to the archive mailbox</span></span>

1. <span data-ttu-id="10536-103">Επιβεβαιώστε ότι έχει ενεργοποιηθεί ένα **γραμματοκιβώτιο αρχειοθέτησης** .</span><span class="sxs-lookup"><span data-stu-id="10536-103">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="10536-104">Εάν όχι, χρησιμοποιήστε τα βήματα [αυτού του άρθρου](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) για να ενεργοποιήσετε το γραμματοκιβώτιο αρχειοθέτησης.</span><span class="sxs-lookup"><span data-stu-id="10536-104">If not, use the steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="10536-105">Για να αρχειοθετήσετε μηνύματα αυτόματα στο γραμματοκιβώτιο αρχειοθέτησης, μια ετικέτα διατήρησης με το **Move για την αρχειοθέτηση** ενέργειας πρέπει να οριστεί να **εφαρμοστεί αυτόματα σε ολόκληρη την ετικέτα γραμματοκιβωτίου (προεπιλογή)**.</span><span class="sxs-lookup"><span data-stu-id="10536-105">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="10536-106">Χρησιμοποιήστε τα βήματα εδώ για να δημιουργήσετε την ετικέτα: [Αρχειοθέτηση προεπιλεγμένη ετικέτα](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="10536-106">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="10536-107">Στη συνέχεια, προσθέστε την ετικέτα **αρχειοθέτησης** στην πολιτική διατήρησης.</span><span class="sxs-lookup"><span data-stu-id="10536-107">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="10536-108">Στο κέντρο διαχείρισης του Exchange, επιλέξτε **πολιτικές διατήρησης** > προσθέσετε την **ετικέτα μετακίνηση στην αρχειοθέτηση** στην πολιτική > **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="10536-108">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="10536-109">Τώρα [Αντιστοιχίστε την πολιτική διατήρησης](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) στο γραμματοκιβώτιο του συγκεκριμένου χρήστη.</span><span class="sxs-lookup"><span data-stu-id="10536-109">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="10536-110">Η ίδια πολιτική θα εφαρμοστεί τόσο στο **πρωτεύον** όσο και στο γραμματοκιβώτιο **αρχειοθέτησης** .</span><span class="sxs-lookup"><span data-stu-id="10536-110">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="10536-111">Μπορεί να είναι απαραίτητο να επιβάλετε το διαχειριζόμενο βοηθό φακέλου (ΣΠΙ) για να εκτελέσετε και να εφαρμόσετε τις νέες ρυθμίσεις στο γραμματοκιβώτιο του χρήστη.</span><span class="sxs-lookup"><span data-stu-id="10536-111">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="10536-112">Εκτελέστε την ακόλουθη εντολή, ενώ έχετε [συνδεθεί με έξω PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) για να ξεκινήσετε το διαχειριζόμενο βοηθό φακέλου για ένα συγκεκριμένο γραμματοκιβώτιο:</span><span class="sxs-lookup"><span data-stu-id="10536-112">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="10536-113">Βοηθός φακέλου-αρχή διαχείρισης-ταυτότητα<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="10536-113">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="10536-114">Για περισσότερες πληροφορίες σχετικά με τη ρύθμιση μιας πολιτικής αρχειοθέτησης, ανατρέξτε στο στοιχείο [ρύθμιση πολιτικής αρχειοθέτησης και διαγραφής για γραμματοκιβώτια](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="10536-114">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  