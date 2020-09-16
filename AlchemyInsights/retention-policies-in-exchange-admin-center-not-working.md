---
title: Οι πολιτικές διατήρησης στο κέντρο διαχείρισης του Exchange δεν λειτουργούν
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 1fee2361b2dd6e0989d430a17aebb13bd5948578
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740510"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="dfa30-102">Πολιτικές διατήρησης στο κέντρο διαχείρισης του Exchange</span><span class="sxs-lookup"><span data-stu-id="dfa30-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="dfa30-103">Εάν θέλετε να εκτελέσουμε αυτοματοποιημένους ελέγχους για τις ρυθμίσεις που αναφέρονται παρακάτω, επιλέξτε το κουμπί πίσω <--στο επάνω μέρος αυτής της σελίδας και, στη συνέχεια, πληκτρολογήστε τη διεύθυνση ηλεκτρονικού ταχυδρομείου του χρήστη που έχει προβλήματα με τις πολιτικές διατήρησης.</span><span class="sxs-lookup"><span data-stu-id="dfa30-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

 <span data-ttu-id="dfa30-104">**Πρόβλημα:** Οι πρόσφατα δημιουργημένες ή ενημερωμένες πολιτικές διατήρησης στο κέντρο διαχείρισης του Exchange δεν εφαρμόζονται σε γραμματοκιβώτια ή τα στοιχεία δεν μετακινούνται στο γραμματοκιβώτιο αρχειοθέτησης ή διαγράφονται.</span><span class="sxs-lookup"><span data-stu-id="dfa30-104">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="dfa30-105">**Ριζικές αιτίες:**</span><span class="sxs-lookup"><span data-stu-id="dfa30-105">**Root Causes:**</span></span>
  
- <span data-ttu-id="dfa30-106">Αυτό μπορεί να συμβαίνει επειδή ο **Βοηθός διαχειριζόμενου φακέλου** δεν έχει επεξεργαστεί το γραμματοκιβώτιο του χρήστη.</span><span class="sxs-lookup"><span data-stu-id="dfa30-106">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="dfa30-107">Ο βοηθός διαχειριζόμενου φακέλου επιχειρεί να επεξεργαστεί κάθε γραμματοκιβώτιο στον οργανισμό σας που βασίζεται στο cloud μία φορά κάθε επτά ημέρες.</span><span class="sxs-lookup"><span data-stu-id="dfa30-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="dfa30-108">Εάν αλλάξετε μια ετικέτα διατήρησης ή εφαρμόζετε μια διαφορετική πολιτική διατήρησης σε ένα γραμματοκιβώτιο, μπορείτε να περιμένετε μέχρι ο διαχειριζόμενος φάκελος να βοηθήσει την επεξεργασία του γραμματοκιβωτίου ή μπορείτε να εκτελέσετε το cmdlet εκκίνησης-ManagedFolderAssistant για να ξεκινήσετε τον βοηθό διαχειριζόμενου φακέλου για να επεξεργαστείτε ένα συγκεκριμένο γραμματοκιβώτιο.</span><span class="sxs-lookup"><span data-stu-id="dfa30-108">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="dfa30-109">Η εκτέλεση αυτού του cmdlet είναι χρήσιμη για τον έλεγχο ή την αντιμετώπιση προβλημάτων μιας πολιτικής διατήρησης ή ρυθμίσεων ετικετών διατήρησης.</span><span class="sxs-lookup"><span data-stu-id="dfa30-109">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="dfa30-110">Για περισσότερες πληροφορίες, επισκεφθείτε [την εκτέλεση του βοηθού διαχειριζόμενου φακέλου](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="dfa30-110">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="dfa30-111">**Λύση:** Εκτελέστε την ακόλουθη εντολή για να ξεκινήσετε το βοηθό διαχειριζόμενου φακέλου για ένα συγκεκριμένο γραμματοκιβώτιο:</span><span class="sxs-lookup"><span data-stu-id="dfa30-111">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="dfa30-112">Αυτό μπορεί επίσης να προκύψει εάν το **RetentionHold** έχει **ενεργοποιηθεί** στο γραμματοκιβώτιο.</span><span class="sxs-lookup"><span data-stu-id="dfa30-112">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="dfa30-113">Εάν το γραμματοκιβώτιο έχει τοποθετηθεί σε ένα RetentionHold, η πολιτική διατήρησης στο γραμματοκιβώτιο δεν θα υποβληθεί σε επεξεργασία στη διάρκεια αυτού του χρόνου.</span><span class="sxs-lookup"><span data-stu-id="dfa30-113">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="dfa30-114">Για περισσότερες informaton στη ρύθμιση RetentionHold, ανατρέξτε στο θέμα: [διατήρηση διατήρησης γραμματοκιβωτίου](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="dfa30-114">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="dfa30-115">**Λύση**</span><span class="sxs-lookup"><span data-stu-id="dfa30-115">**Solution:**</span></span>
    
  - <span data-ttu-id="dfa30-116">Επιλέξτε την κατάσταση της ρύθμισης RetentionHold στο συγκεκριμένο γραμματοκιβώτιο στο [έξω PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="dfa30-116">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="dfa30-117">Εκτελέστε την ακόλουθη εντολή για να **απενεργοποιήσετε** το RetentionHold σε ένα συγκεκριμένο γραμματοκιβώτιο:</span><span class="sxs-lookup"><span data-stu-id="dfa30-117">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="dfa30-118">Τώρα, εκτελέστε ξανά το βοηθό διαχειριζόμενου φακέλου:</span><span class="sxs-lookup"><span data-stu-id="dfa30-118">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="dfa30-119">**Σημείωση:** Εάν ένα γραμματοκιβώτιο είναι μικρότερο από 10 MB, ο διαχειριζόμενος Βοηθός φακέλου δεν θα επεξεργαστεί αυτόματα το γραμματοκιβώτιο.</span><span class="sxs-lookup"><span data-stu-id="dfa30-119">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="dfa30-120">Για περισσότερες πληροφορίες σχετικά με τις πολιτικές διατήρησης στο κέντρο διαχείρισης του Exchange, ανατρέξτε στα θέματα:</span><span class="sxs-lookup"><span data-stu-id="dfa30-120">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="dfa30-121">Ετικέτες διατήρησης και πολιτικές διατήρησης</span><span class="sxs-lookup"><span data-stu-id="dfa30-121">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="dfa30-122">Εφαρμογή πολιτικής διατήρησης σε γραμματοκιβώτια</span><span class="sxs-lookup"><span data-stu-id="dfa30-122">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="dfa30-123">Προσθήκη ή κατάργηση ετικετών διατήρησης</span><span class="sxs-lookup"><span data-stu-id="dfa30-123">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="dfa30-124">Πώς μπορείτε να προσδιορίσετε τον τύπο της διατήρησης που τοποθετείται σε ένα γραμματοκιβώτιο</span><span class="sxs-lookup"><span data-stu-id="dfa30-124">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
