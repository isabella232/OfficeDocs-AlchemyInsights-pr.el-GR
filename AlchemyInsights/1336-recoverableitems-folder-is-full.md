---
title: 1336 RecoverableItems φάκελος είναι πλήρης
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: ee96abfa179c36ebaf43dbd327d4608b849395d3
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29471154"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="39d8f-102">Ο φάκελος στοιχείων με δυνατότητα ανάκτησης είναι πλήρης</span><span class="sxs-lookup"><span data-stu-id="39d8f-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="39d8f-p101">Για τα γραμματοκιβώτια Exchange Online στο Office 365, το προεπιλεγμένο όριο αποθήκευσης για το φάκελο στοιχείων με δυνατότητα ανάκτησης είναι 30 GB. Το όριο αποθήκευσης για το φάκελο στοιχείων με δυνατότητα ανάκτησης αυτόματα αυξάνεται σε 100 GB, εάν το γραμματοκιβώτιο είναι τοποθετημένο σε δίκες κρατήστε, ηλεκτρονική ανακάλυψη αναμονή, ή έχει αντιστοιχιστεί μια πολιτική διατήρησης του Office 365.</span><span class="sxs-lookup"><span data-stu-id="39d8f-p101">For Exchange Online mailboxes in Office 365, the default storage limit for the Recoverable Items folder is 30 GB. The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to an Office 365 retention policy.</span></span>
  
<span data-ttu-id="39d8f-105">Όταν ο φάκελος στοιχείων με δυνατότητα ανάκτησης φτάσει το όριο αποθήκευσης, λειτουργία γραμματοκιβωτίου επηρεάζεται με τους εξής τρόπους:</span><span class="sxs-lookup"><span data-stu-id="39d8f-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>
  
- <span data-ttu-id="39d8f-106">Ο χρήστης δεν είναι δυνατό να διαγράψετε στοιχεία από το γραμματοκιβώτιο.</span><span class="sxs-lookup"><span data-stu-id="39d8f-106">The user can't delete items from the mailbox.</span></span>
    
- <span data-ttu-id="39d8f-107">Διαχείριση Βοηθός φακέλου δεν είναι δυνατό να διαγράψετε στοιχεία που βασίζονται σε tag διατήρησης ή ρυθμίσεις διαχείρισης φακέλων.</span><span class="sxs-lookup"><span data-stu-id="39d8f-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>
    
- <span data-ttu-id="39d8f-108">Για τα γραμματοκιβώτια που έχουν ενεργοποιημένη τη δυνατότητα ανάκτησης στοιχείο μόνο ή τοποθετούνται σε αναμονή, η διαδικασία προστασίας αντιγραφής κατά την εγγραφή σελίδας δεν θα διατηρήσει εκδόσεις των στοιχείων που έχουν υποστεί επεξεργασία από το χρήστη.</span><span class="sxs-lookup"><span data-stu-id="39d8f-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>
    
- <span data-ttu-id="39d8f-109">Για τα γραμματοκιβώτια που διαθέτει γραμματοκιβώτιο καταγραφή ενεργοποιημένη ελέγχου, μπορούν να αποθηκευτούν καταχωρήσεις καταγραφής ελέγχου γραμματοκιβωτίου στον υποφάκελο ελέγχων στο φάκελο στοιχείων με δυνατότητα ανάκτησης.</span><span class="sxs-lookup"><span data-stu-id="39d8f-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>
    
<span data-ttu-id="39d8f-p102">Για τα γραμματοκιβώτια που δεν είναι σε αναμονή, να χρησιμοποιήσετε το "διαχειριστές" της `Search-Mailbox -SearchDumpsterOnly -DeleteContent` εντολή στο Exchange Online PowerShell για να διαγράψετε στοιχεία στο φάκελο στοιχείων με δυνατότητα ανάκτησης. Για περισσότερες πληροφορίες, ανατρέξτε στα παρακάτω θέματα:</span><span class="sxs-lookup"><span data-stu-id="39d8f-p102">For mailboxes that aren't on hold, admins can use the  `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder. For more information, see the following topics:</span></span> 
  
- [<span data-ttu-id="39d8f-112">Αναζητήστε και διαγράψτε μηνύματα</span><span class="sxs-lookup"><span data-stu-id="39d8f-112">Search for and delete messages</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)
    
- [<span data-ttu-id="39d8f-113">Αναζήτηση-γραμματοκιβώτιο</span><span class="sxs-lookup"><span data-stu-id="39d8f-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)
    
<span data-ttu-id="39d8f-p103">Για τα γραμματοκιβώτια που βρίσκονται σε αναμονή, διαχειριστών πρέπει να καταργήσετε τη διατήρηση, πριν να μπορούν να τα διαγραμμένα στοιχεία από το φάκελο στοιχείων με δυνατότητα ανάκτησης. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Διαγραφή στοιχείων από το φάκελο της βασίζεται στο νέφος γραμματοκιβώτια σε κρατήστε στοιχείων με δυνατότητα ανάκτησης](https://docs.microsoft.com/en-us/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="39d8f-p103">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder. For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/en-us/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>
  
<span data-ttu-id="39d8f-p104">Για να αποτρέψετε τη πλήρη φάκελο στοιχείων με δυνατότητα ανάκτησης, "διαχειριστές" μπορεί να αυξήσει το όριο αποθήκευσης του στοιχείων με δυνατότητα ανάκτησης φακέλων για τα γραμματοκιβώτια σε κρατήστε και ορίστε μια πολιτική διατήρησης γραμματοκιβωτίου που μετακινεί τα στοιχεία από το φάκελο στοιχείων με δυνατότητα ανάκτησης σε αρχείο αρχειοθέτησης του χρήστη γραμματοκιβώτιο. Δείτε [αυξήσετε το στόχο για γραμματοκιβώτια κρατήστε στοιχείων με δυνατότητα ανάκτησης](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="39d8f-p104">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox. See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
  

