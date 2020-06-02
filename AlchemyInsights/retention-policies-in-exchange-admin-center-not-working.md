---
title: Οι πολιτικές διατήρησης στο Κέντρο διαχείρισης του Exchange δεν λειτουργούν
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 3040365b9d686bcbcce60977ee9bdbbaffc70b24
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44502607"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="39deb-102">Πολιτικές διατήρησης στο Κέντρο διαχείρισης του Exchange</span><span class="sxs-lookup"><span data-stu-id="39deb-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="39deb-103">**Το θέμα:** Οι νέες πολιτικές διατήρησης που δημιουργήθηκαν πρόσφατα στο Κέντρο διαχείρισης του Exchange δεν εφαρμόζονται σε γραμματοκιβώτια ή τα στοιχεία δεν μετακινούνται στο γραμματοκιβώτιο αρχειοθέτησης ή διαγράφονται.</span><span class="sxs-lookup"><span data-stu-id="39deb-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="39deb-104">**Βασικές αιτίες:**</span><span class="sxs-lookup"><span data-stu-id="39deb-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="39deb-105">Αυτό μπορεί να συμβαίνει επειδή ο **Βοηθός διαχειριζόμενου φακέλου** δεν έχει επεξεργαστεί το γραμματοκιβώτιο του χρήστη.</span><span class="sxs-lookup"><span data-stu-id="39deb-105">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="39deb-106">Ο Βοηθός διαχειριζόμενου φακέλου προσπαθεί να επεξεργαστεί κάθε γραμματοκιβώτιο στον οργανισμό σας που βασίζεται στο cloud μία φορά κάθε επτά ημέρες.</span><span class="sxs-lookup"><span data-stu-id="39deb-106">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="39deb-107">Εάν αλλάξετε μια ετικέτα διατήρησης ή εφαρμόσετε μια διαφορετική πολιτική διατήρησης σε ένα γραμματοκιβώτιο, μπορείτε να περιμένετε μέχρι το Πρόγραμμα υποβοήθησης διαχειριζόμενου φακέλου να επεξεργαστεί το γραμματοκιβώτιο ή μπορείτε να εκτελέσετε το cmdlet Start-ManagedFolderAssistant για να ξεκινήσετε το Βοηθό διαχειριζόμενου φακέλου για να επεξεργαστείτε ένα συγκεκριμένο γραμματοκιβώτιο.</span><span class="sxs-lookup"><span data-stu-id="39deb-107">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="39deb-108">Η εκτέλεση αυτού του cmdlet είναι χρήσιμη για τον έλεγχο ή την αντιμετώπιση προβλημάτων μιας πολιτικής διατήρησης ή ρυθμίσεων ετικέτας διατήρησης.</span><span class="sxs-lookup"><span data-stu-id="39deb-108">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="39deb-109">Για περισσότερες πληροφορίες, [επισκεφθείτε την επιλογή Εκτέλεση του Βοηθού διαχειριζόμενου φακέλου](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="39deb-109">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="39deb-110">**Η λύση:** Εκτελέστε την ακόλουθη εντολή για να ξεκινήσετε το Βοηθό διαχειριζόμενου φακέλου για ένα συγκεκριμένο γραμματοκιβώτιο:</span><span class="sxs-lookup"><span data-stu-id="39deb-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="39deb-111">Αυτό μπορεί επίσης να συμβεί εάν **το RetentionHold** έχει **ενεργοποιηθεί** στο γραμματοκιβώτιο.</span><span class="sxs-lookup"><span data-stu-id="39deb-111">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="39deb-112">Εάν το γραμματοκιβώτιο έχει τοποθετηθεί σε ένα RetentionHold, η πολιτική διατήρησης στο γραμματοκιβώτιο δεν θα υποβληθεί σε επεξεργασία κατά τη διάρκεια αυτής της περιόδου.</span><span class="sxs-lookup"><span data-stu-id="39deb-112">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="39deb-113">Για περισσότερες πληροφορίες σχετικά με τη ρύθμιση Διατήρηση διατήρησης, ανατρέξτε [στο θέμα: Διατήρηση γραμματοκιβωτίου Διατήρηση .](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)</span><span class="sxs-lookup"><span data-stu-id="39deb-113">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="39deb-114">**Λύση:**</span><span class="sxs-lookup"><span data-stu-id="39deb-114">**Solution:**</span></span>
    
  - <span data-ttu-id="39deb-115">Ελέγξτε την κατάσταση της ρύθμισης Διατήρηση διατήρησης στο συγκεκριμένο γραμματοκιβώτιο στο [powershell EXO](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="39deb-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="39deb-116">Εκτελέστε την ακόλουθη εντολή για να **απενεργοποιήσετε** το RetentionHold σε ένα συγκεκριμένο γραμματοκιβώτιο:</span><span class="sxs-lookup"><span data-stu-id="39deb-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="39deb-117">Τώρα, εκτελέστε εκ νέου το Βοηθό διαχειριζόμενου φακέλου:</span><span class="sxs-lookup"><span data-stu-id="39deb-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="39deb-118">**Σημείωση:** Εάν ένα γραμματοκιβώτιο είναι μικρότερο από 10 MB, ο Βοηθός διαχειριζόμενου φακέλου δεν θα επεξεργαστεί αυτόματα το γραμματοκιβώτιο.</span><span class="sxs-lookup"><span data-stu-id="39deb-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="39deb-119">Για περισσότερες πληροφορίες σχετικά με τις πολιτικές διατήρησης στο Κέντρο διαχείρισης του Exchange, ανατρέξτε στα θέματα:</span><span class="sxs-lookup"><span data-stu-id="39deb-119">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="39deb-120">Ετικέτες διατήρησης και πολιτικές διατήρησης</span><span class="sxs-lookup"><span data-stu-id="39deb-120">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="39deb-121">Εφαρμογή πολιτικής διατήρησης σε γραμματοκιβώτια</span><span class="sxs-lookup"><span data-stu-id="39deb-121">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="39deb-122">Προσθήκη ή κατάργηση ετικετών διατήρησης</span><span class="sxs-lookup"><span data-stu-id="39deb-122">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="39deb-123">Τρόπος αναγνώρισης του τύπου διατήρησης που τοποθετείται σε ένα γραμματοκιβώτιο</span><span class="sxs-lookup"><span data-stu-id="39deb-123">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
