---
title: 1336 Ο φάκελος RecoverableItems είναι πλήρης
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: fb10b792981040bdcf4661b8aff30733c2438212
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720252"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="12ab8-102">Ο φάκελος "Ανακτήσιμα στοιχεία" είναι πλήρης</span><span class="sxs-lookup"><span data-stu-id="12ab8-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="12ab8-103">Για γραμματοκιβώτια του Exchange Online, το προεπιλεγμένο όριο χώρου αποθήκευσης για το φάκελο "Ανακτήσιμα στοιχεία" είναι 30 GB.</span><span class="sxs-lookup"><span data-stu-id="12ab8-103">For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="12ab8-104">Το όριο αποθήκευσης για το φάκελο "Ανακτήσιμα στοιχεία" αυξάνεται αυτόματα στα 100 GB, εάν το γραμματοκιβώτιο έχει τοποθετηθεί σε διατήρηση διαφορών, διατήρηση eDiscovery ή αντιστοιχιστεί σε μια πολιτική διατήρησης.</span><span class="sxs-lookup"><span data-stu-id="12ab8-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to a retention policy.</span></span>

<span data-ttu-id="12ab8-105">Όταν ο φάκελος "Ανακτήσιμα στοιχεία" φτάσει στο όριο αποθήκευσης, η λειτουργικότητα του γραμματοκιβωτίου επηρεάζεται με τους ακόλουθους τρόπους:</span><span class="sxs-lookup"><span data-stu-id="12ab8-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="12ab8-106">Ο χρήστης δεν είναι δυνατό να διαγράψει στοιχεία από το γραμματοκιβώτιο.</span><span class="sxs-lookup"><span data-stu-id="12ab8-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="12ab8-107">Ο Βοηθός διαχειριζόμενου φακέλου δεν είναι δυνατό να διαγράψει στοιχεία με βάση την ετικέτα διατήρησης ή τις ρυθμίσεις διαχειριζόμενου φακέλου.</span><span class="sxs-lookup"><span data-stu-id="12ab8-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="12ab8-108">Για γραμματοκιβώτια που έχουν ενεργοποιημένη την Ανάκτηση ενός στοιχείου ή έχουν τεθεί σε αναμονή, η διαδικασία προστασίας σελίδας αντιγραφής κατά την εγγραφή δεν μπορεί να διατηρήσει εκδόσεις στοιχείων που έχουν υποστεί επεξεργασία από το χρήστη.</span><span class="sxs-lookup"><span data-stu-id="12ab8-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="12ab8-109">Για γραμματοκιβώτια που έχουν ενεργοποιημένη την καταγραφή ελέγχου γραμματοκιβωτίου, δεν είναι δυνατή η αποθήκευση καταχωρήσεων αρχείου καταγραφής ελέγχου γραμματοκιβωτίου στον υποφάκελο "Έλεγχοι" στο φάκελο "Ανακτήσιμα στοιχεία".</span><span class="sxs-lookup"><span data-stu-id="12ab8-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="12ab8-110">Για γραμματοκιβώτια που δεν βρίσκονται σε αναμονή, `Search-Mailbox -SearchDumpsterOnly -DeleteContent` οι διαχειριστές μπορούν να χρησιμοποιήσουν την εντολή στο Exchange Online PowerShell για να διαγράψουν στοιχεία στο φάκελο "Ανακτήσιμα στοιχεία".</span><span class="sxs-lookup"><span data-stu-id="12ab8-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="12ab8-111">Για περισσότερες πληροφορίες, ανατρέξτε στα παρακάτω θέματα:</span><span class="sxs-lookup"><span data-stu-id="12ab8-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="12ab8-112">Αναζήτηση και διαγραφή μηνυμάτων</span><span class="sxs-lookup"><span data-stu-id="12ab8-112">Search for and delete messages</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="12ab8-113">Γραμματοκιβώτιο αναζήτησης</span><span class="sxs-lookup"><span data-stu-id="12ab8-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="12ab8-114">Για γραμματοκιβώτια που βρίσκονται σε αναμονή, οι διαχειριστές πρέπει να καταργήσουν τη διατήρηση για να μπορέσουν να διαγραφούν στοιχεία από το φάκελο "Ανακτήσιμα στοιχεία".</span><span class="sxs-lookup"><span data-stu-id="12ab8-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="12ab8-115">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Διαγραφή στοιχείων στο φάκελο "Ανακτήσιμα στοιχεία" των γραμματοκιβωτίων που βασίζονται στο cloud σε αναμονή](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="12ab8-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="12ab8-116">Για να αποτρέψετε την πλήρη δημιουργία του φακέλου "Ανακτήσιμα στοιχεία", οι διαχειριστές μπορούν να αυξήσουν το όριο αποθήκευσης του φακέλου "Ανακτήσιμα στοιχεία" για γραμματοκιβώτια σε αναμονή και να δημιουργήσουν μια πολιτική διατήρησης γραμματοκιβωτίου που μετακινεί στοιχεία από το φάκελο "Ανακτήσιμα στοιχεία" στο γραμματοκιβώτιο αρχειοθέτησης του χρήστη.</span><span class="sxs-lookup"><span data-stu-id="12ab8-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="12ab8-117">Ανατρέξτε στο θέμα [Αύξηση του ορίου ανακτήσιμων στοιχείων για γραμματοκιβώτια σε αναμονή](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="12ab8-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
