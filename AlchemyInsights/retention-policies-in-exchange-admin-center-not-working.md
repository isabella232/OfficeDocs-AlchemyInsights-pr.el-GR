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
ms.openlocfilehash: 4d3ca121c8d22a0900f136f7f2a754dfb5b435f5
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522807"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="8a2a2-102">Πολιτικές διατήρησης στο Κέντρο διαχείρισης του Exchange</span><span class="sxs-lookup"><span data-stu-id="8a2a2-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="8a2a2-103">Αν θέλετε να εκτελέσουμε αυτοματοποιημένους ελέγχους για τις ρυθμίσεις που αναφέρονται παρακάτω, επιλέξτε το κουμπί "Πίσω" <-- στο επάνω μέρος αυτής της σελίδας και, στη συνέχεια, πληκτρολογήστε τη διεύθυνση ηλεκτρονικού ταχυδρομείου του χρήστη που έχει προβλήματα με τις πολιτικές διατήρησης.</span><span class="sxs-lookup"><span data-stu-id="8a2a2-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

 <span data-ttu-id="8a2a2-104">**Τεύχος:** Οι πολιτικές διατήρησης που δημιουργήθηκαν ή ενημερώθηκαν πρόσφατα στο Κέντρο διαχείρισης του Exchange δεν εφαρμόζονται σε γραμματοκιβώτια ή στοιχεία, οι οποίοι δεν μετακινούνται στο γραμματοκιβώτιο αρχειοθέτησης ή δεν διαγράφονται.</span><span class="sxs-lookup"><span data-stu-id="8a2a2-104">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="8a2a2-105">**Ριζικές αιτίες:**</span><span class="sxs-lookup"><span data-stu-id="8a2a2-105">**Root Causes:**</span></span>
  
- <span data-ttu-id="8a2a2-106">Αυτό μπορεί να συμβαίνει επειδή ο **Βοηθός διαχειριζόμενων φακέλων** δεν έχει επεξεργαστεί το γραμματοκιβώτιο του χρήστη.</span><span class="sxs-lookup"><span data-stu-id="8a2a2-106">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="8a2a2-107">Ο Βοηθός διαχειριζόμενων φακέλων προσπαθεί να επεξεργάζεται κάθε γραμματοκιβώτιο στον οργανισμό σας που βασίζεται στο cloud μία φορά κάθε επτά ημέρες.</span><span class="sxs-lookup"><span data-stu-id="8a2a2-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="8a2a2-108">Εάν αλλάξετε μια ετικέτα διατήρησης ή εφαρμόσετε μια διαφορετική πολιτική διατήρησης σε ένα γραμματοκιβώτιο, μπορείτε να περιμένετε μέχρι το Πρόγραμμα βοήθειας διαχειριζόμενου φακέλου να επεξεργαστεί το γραμματοκιβώτιο ή μπορείτε να εκτελέσετε το cmdlet Start-ManagedFolderAssistant για να ξεκινήσετε το Βοηθό διαχειριζόμενων φακέλων για να επεξεργαστείτε ένα συγκεκριμένο γραμματοκιβώτιο.</span><span class="sxs-lookup"><span data-stu-id="8a2a2-108">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="8a2a2-109">Η εκτέλεση αυτού του cmdlet είναι χρήσιμη για τον έλεγχο ή την αντιμετώπιση προβλημάτων μιας πολιτικής διατήρησης ή των ρυθμίσεων ετικέτας διατήρησης.</span><span class="sxs-lookup"><span data-stu-id="8a2a2-109">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="8a2a2-110">Για περισσότερες πληροφορίες, επισκεφθείτε την επιλογή [Εκτέλεση του Βοηθού διαχειριζόμενων φακέλων](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="8a2a2-110">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="8a2a2-111">**Λύση:** Εκτελέστε την ακόλουθη εντολή για να ξεκινήσετε το Βοηθό διαχειριζόμενων φακέλων για ένα συγκεκριμένο γραμματοκιβώτιο:</span><span class="sxs-lookup"><span data-stu-id="8a2a2-111">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="8a2a2-112">Αυτό μπορεί επίσης να συμβεί εάν **το Retendhold** έχει **ενεργοποιηθεί** στο γραμματοκιβώτιο.</span><span class="sxs-lookup"><span data-stu-id="8a2a2-112">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="8a2a2-113">Εάν το γραμματοκιβώτιο έχει τοποθετηθεί σε ένα Retenten that The reten that, η πολιτική διατήρησης στο γραμματοκιβώτιο δεν θα υποβληθεί σε επεξεργασία κατά τη διάρκεια αυτής της περιόδου.</span><span class="sxs-lookup"><span data-stu-id="8a2a2-113">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="8a2a2-114">Για περισσότερες πληροφορίες σχετικά με τη ρύθμιση Retenten παρακρατήστε: [Διατήρηση γραμματοκιβωτίου .](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)</span><span class="sxs-lookup"><span data-stu-id="8a2a2-114">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="8a2a2-115">**Λύση:**</span><span class="sxs-lookup"><span data-stu-id="8a2a2-115">**Solution:**</span></span>
    
  - <span data-ttu-id="8a2a2-116">Ελέγξτε την κατάσταση της ρύθμισης Retenten the retendoiseHold στο συγκεκριμένο γραμματοκιβώτιο στο [powershell EXO](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="8a2a2-116">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="8a2a2-117">Εκτελέστε την ακόλουθη εντολή για να **απενεργοποιήσετε** το Retententen εκ των τες δύο σε ένα συγκεκριμένο γραμματοκιβώτιο:</span><span class="sxs-lookup"><span data-stu-id="8a2a2-117">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="8a2a2-118">Τώρα, εκτελέστε εκ νέου το Βοηθό διαχειριζόμενων φακέλων:</span><span class="sxs-lookup"><span data-stu-id="8a2a2-118">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="8a2a2-119">**Σημείωση:** Εάν ένα γραμματοκιβώτιο είναι μικρότερο από 10 MB, ο Βοηθός διαχειριζόμενων φακέλων δεν θα επεξεργαστεί αυτόματα το γραμματοκιβώτιο.</span><span class="sxs-lookup"><span data-stu-id="8a2a2-119">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="8a2a2-120">Για περισσότερες πληροφορίες σχετικά με τις πολιτικές διατήρησης στο Κέντρο διαχείρισης του Exchange, ανατρέξτε στα θέματα:</span><span class="sxs-lookup"><span data-stu-id="8a2a2-120">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="8a2a2-121">Ετικέτες διατήρησης και πολιτικές διατήρησης</span><span class="sxs-lookup"><span data-stu-id="8a2a2-121">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="8a2a2-122">Εφαρμογή πολιτικής διατήρησης σε γραμματοκιβώτια</span><span class="sxs-lookup"><span data-stu-id="8a2a2-122">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="8a2a2-123">Προσθήκη ή κατάργηση ετικετών διατήρησης</span><span class="sxs-lookup"><span data-stu-id="8a2a2-123">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="8a2a2-124">Τρόπος αναγνώρισης του τύπου διατήρησης που τοποθετείται σε ένα γραμματοκιβώτιο</span><span class="sxs-lookup"><span data-stu-id="8a2a2-124">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
