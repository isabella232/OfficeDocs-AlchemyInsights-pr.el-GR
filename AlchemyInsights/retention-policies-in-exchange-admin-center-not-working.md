---
title: Οι πολιτικές διατήρησης στο Κέντρο διαχείρισης του Exchange δεν λειτουργεί
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 9f4a175239bc20aaf489615da63ef35002030a70
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35369665"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="260e3-102">Οι πολιτικές διατήρησης στο Κέντρο διαχείρισης του Exchange</span><span class="sxs-lookup"><span data-stu-id="260e3-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="260e3-103">**Θέμα:** Που δημιουργήθηκαν πρόσφατα ή πολιτικές διατήρησης ενημερωμένο στο Κέντρο διαχείρισης Exchange δεν εφαρμόζουν γραμματοκιβώτια ή στοιχεία δεν μετακινούνται στο γραμματοκιβώτιο αρχειοθέτηση ή διαγραφή.</span><span class="sxs-lookup"><span data-stu-id="260e3-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="260e3-104">**Βασικές αιτίες:**</span><span class="sxs-lookup"><span data-stu-id="260e3-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="260e3-105">Αυτό μπορεί να οφείλεται η **Διαχείριση Βοηθός φακέλου** δεν επεξεργάστηκε το γραμματοκιβώτιο του χρήστη.</span><span class="sxs-lookup"><span data-stu-id="260e3-105">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="260e3-106">Η διαχείριση Βοηθός φακέλου προσπαθεί να επεξεργαστεί κάθε γραμματοκιβώτιο στον οργανισμό σας βασίζεται στο νέφος μία φορά κάθε επτά ημέρες.</span><span class="sxs-lookup"><span data-stu-id="260e3-106">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="260e3-107">Εάν αλλάξετε μια ετικέτα διατήρησης ή εφαρμόζεται διαφορετική πολιτική διατήρησης σε ένα γραμματοκιβώτιο, μπορείτε να περιμένετε μέχρι η διαχειριζόμενη φάκελο επικουρεί επεξεργάζεται το γραμματοκιβώτιο, ή μπορείτε να εκτελέσετε το cmdlet έναρξης-ManagedFolderAssistant για να ξεκινήσετε τη Διαχείριση Βοηθός φακέλου για να επεξεργαστείτε μια συγκεκριμένη γραμματοκιβώτιο.</span><span class="sxs-lookup"><span data-stu-id="260e3-107">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="260e3-108">Εκτέλεση αυτού του cmdlet είναι χρήσιμη για τη δοκιμή ή την αντιμετώπιση προβλημάτων μια πολιτική διατήρησης ή ρυθμίσεις ετικέτα διατήρησης.</span><span class="sxs-lookup"><span data-stu-id="260e3-108">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="260e3-109">Για περισσότερες πληροφορίες, επισκεφθείτε την [Εκτέλεση διαχειριζόμενου Βοηθός φακέλου](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="260e3-109">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="260e3-110">**Λύση:** Εκτελέστε την ακόλουθη εντολή για να ξεκινήσετε τη Διαχείριση Βοηθός φακέλου για ένα συγκεκριμένο γραμματοκιβώτιο:</span><span class="sxs-lookup"><span data-stu-id="260e3-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="260e3-111">Αυτό μπορεί να συμβεί επίσης αν **RetentionHold** έχει **ενεργοποιηθεί** στο γραμματοκιβώτιο.</span><span class="sxs-lookup"><span data-stu-id="260e3-111">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="260e3-112">Εάν το γραμματοκιβώτιο έχει τοποθετηθεί σε ένα RetentionHold, δεν θα γίνει επεξεργασία της πολιτικής διατήρησης στο γραμματοκιβώτιο σε αυτό το διάστημα.</span><span class="sxs-lookup"><span data-stu-id="260e3-112">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="260e3-113">Για περισσότερες informaton, δείτε: ρύθμιση της RetentionHold: [Κρατήστε διατήρησης γραμματοκιβωτίου](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="260e3-113">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="260e3-114">**Λύση:**</span><span class="sxs-lookup"><span data-stu-id="260e3-114">**Solution:**</span></span>
    
  - <span data-ttu-id="260e3-115">Ελέγξτε την κατάσταση της ρύθμισης RetentionHold στο συγκεκριμένο γραμματοκιβώτιο σε [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="260e3-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="260e3-116">Εκτελέστε την ακόλουθη εντολή για να **απενεργοποιήσετε** RetentionHold για ένα συγκεκριμένο γραμματοκιβώτιο:</span><span class="sxs-lookup"><span data-stu-id="260e3-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="260e3-117">Τώρα, εκτελέστε ξανά το φάκελο διαχειριζόμενες Βοηθός:</span><span class="sxs-lookup"><span data-stu-id="260e3-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="260e3-118">**Σημείωση:** Εάν ένα γραμματοκιβώτιο είναι μικρότερο από 10 MB, η διαχείριση Βοηθός φακέλου θα γίνει αυτόματα επεξεργασία στο γραμματοκιβώτιο.</span><span class="sxs-lookup"><span data-stu-id="260e3-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
  