---
title: ο φάκελος RecoverableItems του 1336 είναι πλήρης
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
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 6ae608b776332402fe333315f5e4ff6072b0a651
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741267"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="0d53b-102">Ο φάκελος "ανακτήσιμα στοιχεία" είναι γεμάτος</span><span class="sxs-lookup"><span data-stu-id="0d53b-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="0d53b-103">Για τα γραμματοκιβώτια του Exchange Online, το προεπιλεγμένο όριο χώρου αποθήκευσης για το φάκελο "ανακτήσιμα στοιχεία" είναι 30 GB.</span><span class="sxs-lookup"><span data-stu-id="0d53b-103">For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="0d53b-104">Το όριο χώρου αποθήκευσης για το φάκελο "ανακτήσιμα στοιχεία" αυξάνεται αυτόματα σε 100 GB, εάν το γραμματοκιβώτιο τοποθετείται σε αναμονή εκδίκασης διαφορών, διατήρηση ανακάλυψης ή έχει αντιστοιχιστεί σε μια πολιτική διατήρησης.</span><span class="sxs-lookup"><span data-stu-id="0d53b-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to a retention policy.</span></span>

<span data-ttu-id="0d53b-105">Όταν ο φάκελος "ανακτήσιμα στοιχεία" φθάσει στο όριο χώρου αποθήκευσης, η λειτουργικότητα του γραμματοκιβωτίου επηρεάζεται με τους εξής τρόπους:</span><span class="sxs-lookup"><span data-stu-id="0d53b-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="0d53b-106">Ο χρήστης δεν μπορεί να διαγράψει στοιχεία από το γραμματοκιβώτιο.</span><span class="sxs-lookup"><span data-stu-id="0d53b-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="0d53b-107">Ο βοηθός διαχειριζόμενου φακέλου δεν μπορεί να διαγράψει στοιχεία με βάση την ετικέτα διατήρησης ή τις ρυθμίσεις διαχειριζόμενου φακέλου.</span><span class="sxs-lookup"><span data-stu-id="0d53b-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="0d53b-108">Για τα γραμματοκιβώτια που έχουν ενεργοποιημένη την ανάκτηση ενός στοιχείου ή τοποθετούνται σε αναμονή, η διαδικασία προστασίας της σελίδας αντιγραφής-εγγραφής δεν μπορεί να διατηρήσει τις εκδόσεις των στοιχείων που επεξεργάστηκε ο χρήστης.</span><span class="sxs-lookup"><span data-stu-id="0d53b-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="0d53b-109">Για τα γραμματοκιβώτια που έχουν ενεργοποιημένη την καταγραφή ελέγχου γραμματοκιβωτίου, δεν είναι δυνατή η αποθήκευση καταχωρήσεων του αρχείου καταγραφής ελέγχου γραμματοκιβωτίου στον υποφάκελο "ελεγκτές" στο φάκελο "ανακτήσιμα στοιχεία".</span><span class="sxs-lookup"><span data-stu-id="0d53b-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="0d53b-110">Για τα γραμματοκιβώτια που δεν βρίσκονται σε αναμονή, οι διαχειριστές μπορούν να χρησιμοποιήσουν την `Search-Mailbox -SearchDumpsterOnly -DeleteContent` εντολή στο Exchange Online PowerShell για να διαγράψουν στοιχεία στο φάκελο ανακτήσιμα στοιχεία.</span><span class="sxs-lookup"><span data-stu-id="0d53b-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="0d53b-111">Για περισσότερες πληροφορίες, ανατρέξτε στα παρακάτω θέματα:</span><span class="sxs-lookup"><span data-stu-id="0d53b-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="0d53b-112">Αναζήτηση και διαγραφή μηνυμάτων</span><span class="sxs-lookup"><span data-stu-id="0d53b-112">Search for and delete messages</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="0d53b-113">Αναζήτηση-γραμματοκιβώτιο</span><span class="sxs-lookup"><span data-stu-id="0d53b-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="0d53b-114">Για τα γραμματοκιβώτια που βρίσκονται σε αναμονή, οι διαχειριστές πρέπει να αφαιρέσουν την αναμονή για να μπορέσουν να διαγραφούν στοιχεία από το φάκελο "ανακτήσιμα στοιχεία".</span><span class="sxs-lookup"><span data-stu-id="0d53b-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="0d53b-115">Για περισσότερες πληροφορίες, ανατρέξτε στο [θέμα Διαγραφή στοιχείων στο φάκελο "ανακτήσιμα στοιχεία" των γραμματοκιβωτίων που βασίζονται στο cloud σε αναμονή](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="0d53b-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="0d53b-116">Για να αποτρέψετε την πλήρη εκκαθάριση του φακέλου "ανακτήσιμα στοιχεία", οι διαχειριστές μπορούν να αυξήσουν το όριο χώρου αποθήκευσης του φακέλου "ανακτήσιμα στοιχεία" για τα γραμματοκιβώτια σε αναμονή και να ορίσουν μια πολιτική διατήρησης γραμματοκιβωτίου που μετακινεί στοιχεία από το φάκελο "ανακτήσιμα στοιχεία" στο γραμματοκιβώτιο αρχειοθέτησης του χρήστη.</span><span class="sxs-lookup"><span data-stu-id="0d53b-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="0d53b-117">Ανατρέξτε [στο θέμα αύξηση του ορίου ανακτήσιμων στοιχείων για τα γραμματοκιβώτια σε αναμονή](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="0d53b-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
