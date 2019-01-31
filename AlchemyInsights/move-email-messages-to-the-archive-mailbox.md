---
title: Μετακίνηση μηνυμάτων ηλεκτρονικού ταχυδρομείου στο γραμματοκιβώτιο αρχειοθέτησης
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 2147c70f64087bf95fc4e39c193caeac3b2c5361
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29660379"
---
<span data-ttu-id="74764-p101">Αντιμετωπίζετε προβλήματα Αρχειοθέτηση στοιχείων στο γραμματοκιβώτιο αρχειοθέτησης. Βεβαιωθείτε ότι έχετε εκτελέσει τα παρακάτω βήματα:</span><span class="sxs-lookup"><span data-stu-id="74764-p101">Having problems archiving items to the Archive mailbox. Make sure you have performed the following steps:</span></span>
  
1. <span data-ttu-id="74764-p102">Επιβεβαιώστε ότι μια **Αρχειοθέτηση γραμματοκιβώτιο** έχει ενεργοποιηθεί. Εάν όχι, χρησιμοποιήστε τα βήματα σε [αυτό το άρθρο](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) , για να ενεργοποιήσετε το γραμματοκιβώτιο αρχειοθέτησης.</span><span class="sxs-lookup"><span data-stu-id="74764-p102">Confirm that an **Archive mailbox** has been enabled. If not, use steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span> 
    
2. <span data-ttu-id="74764-106">Στο Κέντρο διαχείρισης Exchange, επιλέξτε **Ετικέτες διατήρησης** στην περιοχή **Διαχείριση συμμόρφωσης**, δημιουργήστε μια **ετικέτα διατήρησης** με την ενέργεια **μετακινήσετε σε αρχείο αρχειοθέτησης** που περιέχει την επιθυμητή **Ηλικία διατήρησης**.</span><span class="sxs-lookup"><span data-stu-id="74764-106">In the Exchange Admin Center, select **Retention Tags** under **Compliance Management**, create a **Retention tag** with the **Move to Archive** action containing the desired **Retention Age**.</span></span>
    
3. <span data-ttu-id="74764-107">Στο Κέντρο διαχείρισης Exchange, επιλέξτε **Πολιτικές διατήρησης**, δημιουργήστε μια **Πολιτική διατήρησης** και προσθέστε την ετικέτα διατήρησης **προς φύλαξη** συγκεκριμένη πολιτική.</span><span class="sxs-lookup"><span data-stu-id="74764-107">In the Exchange Admin Center, select **Retention Policies**, create a **Retention Policy** and add your **Move to Archive** retention tag to that policy.</span></span> 
    
4. <span data-ttu-id="74764-p103">[Εκχώρηση της πολιτικής διατήρησης](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) στο γραμματοκιβώτιο του συγκεκριμένου χρήστη. Την ίδια πολιτική θα εφαρμοστεί για το **πρωτεύον** και το γραμματοκιβώτιο **αρχειοθέτησης** .</span><span class="sxs-lookup"><span data-stu-id="74764-p103">[Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox. The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span> 
    
<span data-ttu-id="74764-p104">Το γραμματοκιβώτιο του χρήστη θα πρέπει τώρα να έχετε μια πολιτική αρχειοθέτησης για τη μετακίνηση στοιχείων στο γραμματοκιβώτιο αρχειοθέτησης. Μπορεί να είναι απαραίτητο για να εξαναγκαστεί διαχειριζόμενη φάκελο Βοηθός (ΣΠΙ) για να εκτελέσετε και να εφαρμόσετε τις νέες ρυθμίσεις για το γραμματοκιβώτιο του χρήστη. Εκτελέστε την ακόλουθη εντολή ενώ [συνδεδεμένοι EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) για να ξεκινήσετε τη Διαχείριση Βοηθός φακέλου για ένα συγκεκριμένο γραμματοκιβώτιο:</span><span class="sxs-lookup"><span data-stu-id="74764-p104">The user's mailbox should now have an Archive policy to move items to the Archive mailbox. It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox. Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span> 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

<span data-ttu-id="74764-113">Θέλετε περισσότερες πληροφορίες σχετικά με τη διαμόρφωση πολιτικής αρχειοθέτησης, ανατρέξτε στο θέμα [Ρύθμιση μιας πολιτικής αρχειοθέτησης και διαγραφής για τα γραμματοκιβώτια](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="74764-113">Want more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  

