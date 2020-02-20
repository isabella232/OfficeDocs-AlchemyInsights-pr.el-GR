---
title: Συνταξιοδότηση των εργαλείων ανακάλυψης παλαιού τύπου
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: c4632b52dde579b7d5b2e6e15f1583300a0bd136
ms.sourcegitcommit: a7c17217c170ead24571421baaf5a14f1525b1a6
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42157596"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="7f882-102">Συνταξιοδότηση των εργαλείων ανακάλυψης παλαιού τύπου</span><span class="sxs-lookup"><span data-stu-id="7f882-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="7f882-103">Ως αποτέλεσμα της νέας και βελτιωμένης λειτουργίας ανακάλυψης στο κέντρο συμμόρφωσης της Microsoft 365, τα ακόλουθα εργαλεία ανακάλυψης παλαιού τύπου και commandlets θα αποσυρθεί κατά τους επόμενους μήνες:</span><span class="sxs-lookup"><span data-stu-id="7f882-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="7f882-104">[Επιτόπου ανακάλυψης](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) και [επιτόπου κατέχει](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) στο κέντρο διαχείρισης του Exchange.</span><span class="sxs-lookup"><span data-stu-id="7f882-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="7f882-105">Το Exchange Online PowerShell cmdlets που υποστηρίζουν επιτόπου ανακάλυψης και επιτόπου κατέχει.</span><span class="sxs-lookup"><span data-stu-id="7f882-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="7f882-106">(Αυτά τα cmdlets αναγνωρίζονται συλλογικά ως \*-MailboxSearch cmdlets.) Αυτό περιλαμβάνει τα ακόλουθα cmdlets:</span><span class="sxs-lookup"><span data-stu-id="7f882-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="7f882-107">ΝΕΟ-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="7f882-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="7f882-108">Έναρξη-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="7f882-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="7f882-109">Stop-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="7f882-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="7f882-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="7f882-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="7f882-111">Το cmdlet [γραμματοκιβώτιο αναζήτησης](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) στο Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="7f882-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="7f882-112">Τις ακόλουθες λειτουργίες στο API των υπηρεσιών Web του Exchange:</span><span class="sxs-lookup"><span data-stu-id="7f882-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="7f882-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="7f882-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="7f882-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="7f882-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="7f882-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="7f882-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="7f882-116">Office 365 προηγμένη ανακάλυψη v 1.0</span><span class="sxs-lookup"><span data-stu-id="7f882-116">Office 365 Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/en-us/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="7f882-117">**Χρονοδιάγραμμα για τη συνταξιοδότηση**:</span><span class="sxs-lookup"><span data-stu-id="7f882-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="7f882-118">1 Απριλίου 2020: δεν θα μπορείτε να δημιουργήσετε νέες αναζητήσεις και να διατηρείτε, αλλά μπορείτε ακόμα να εκτελέσετε, να επεξεργαστείτε και να διαγράψετε υπάρχουσες αναζητήσεις με δική σας ευθύνη.</span><span class="sxs-lookup"><span data-stu-id="7f882-118">April 1, 2020: You won't be able to create new searches and holds, but you can still run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="7f882-119">Η υποστήριξη της Microsoft δεν θα υποστηρίζει πλέον επιτόπου ανακάλυψης & διατηρεί στην ΑΗΚ.</span><span class="sxs-lookup"><span data-stu-id="7f882-119">Microsoft Support will no longer support In-Place eDiscovery & Holds in the EAC.</span></span>

- <span data-ttu-id="7f882-120">1 Ιουλίου 2020: η επιτόπου ανακάλυψης & κατέχει λειτουργικότητα στην ΑΗΚ θα τοποθετηθεί σε λειτουργία μόνο για ανάγνωση.</span><span class="sxs-lookup"><span data-stu-id="7f882-120">July 1, 2020: The In-Place eDiscovery & Holds functionality in the EAC will be placed in a read-only mode.</span></span> <span data-ttu-id="7f882-121">Αυτό σημαίνει ότι θα είστε σε θέση να αφαιρέσετε μόνο τις υπάρχουσες αναζητήσεις και διατηρεί.</span><span class="sxs-lookup"><span data-stu-id="7f882-121">This means you'll only be able to remove existing searches and holds.</span></span>

<span data-ttu-id="7f882-122">**Για περισσότερες πληροφορίες, ανατρέξτε**στο:</span><span class="sxs-lookup"><span data-stu-id="7f882-122">**For more information, see**:</span></span>

 - [<span data-ttu-id="7f882-123">Μετεγκατάσταση αναζητήσεις ανακάλυψης παλαιού τύπου και διατηρεί στο κέντρο συμμόρφωσης Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="7f882-123">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/en-us/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="7f882-124">Συνταξιοδότηση των εργαλείων ανακάλυψης παλαιού τύπου</span><span class="sxs-lookup"><span data-stu-id="7f882-124">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="7f882-125">Συχνές ερωτήσεις σχετικά με την επιτόπου ανακάλυψη και επιτόπου κατέχει</span><span class="sxs-lookup"><span data-stu-id="7f882-125">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



