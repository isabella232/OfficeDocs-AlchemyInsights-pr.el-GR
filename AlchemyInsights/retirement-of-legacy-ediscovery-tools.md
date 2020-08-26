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
ms.openlocfilehash: 94cd2127240be5faacd397ba6255fdb16e364308
ms.sourcegitcommit: d4fc2a03af69e28e96075812d040fdd34d2e23f0
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/26/2020
ms.locfileid: "46902620"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="d97d0-102">Συνταξιοδότηση των εργαλείων ανακάλυψης παλαιού τύπου</span><span class="sxs-lookup"><span data-stu-id="d97d0-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="d97d0-103">Ως αποτέλεσμα της νέας και βελτιωμένης λειτουργικότητας ανακάλυψης στο κέντρο συμμόρφωσης του Microsoft 365, τα παρακάτω εργαλεία ανακάλυψης παλαιού τύπου και τα commandlets θα αποσύρονται τους επόμενους μήνες:</span><span class="sxs-lookup"><span data-stu-id="d97d0-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="d97d0-104">Επιτόπια [ανακάλυψη](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) και [επιτόπου κατοχή](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) στο κέντρο διαχείρισης του Exchange.</span><span class="sxs-lookup"><span data-stu-id="d97d0-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="d97d0-105">Τα cmdlet του Exchange Online PowerShell που υποστηρίζουν την επιτόπια ανακάλυψη και την επιτόπια κατοχή.</span><span class="sxs-lookup"><span data-stu-id="d97d0-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="d97d0-106">(Αυτά τα cmdlets προσδιορίζονται συλλογικά ως \*-MailboxSearch cmdlets.) Αυτό περιλαμβάνει τα ακόλουθα cmdlet:</span><span class="sxs-lookup"><span data-stu-id="d97d0-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="d97d0-107">New-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="d97d0-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="d97d0-108">Έναρξη-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="d97d0-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="d97d0-109">Stop-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="d97d0-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="d97d0-110">Ορίστε-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="d97d0-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="d97d0-111">Το cmdlet του [γραμματοκιβωτίου αναζήτησης](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) στο Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="d97d0-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="d97d0-112">Τις ακόλουθες λειτουργίες στο API των υπηρεσιών Web του Exchange:</span><span class="sxs-lookup"><span data-stu-id="d97d0-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="d97d0-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="d97d0-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="d97d0-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="d97d0-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="d97d0-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="d97d0-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="d97d0-116">Προηγμένη ηλεκτρονική ανακάλυψη v 1.0</span><span class="sxs-lookup"><span data-stu-id="d97d0-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="d97d0-117">**Λωρίδα χρόνου για συνταξιοδότηση**:</span><span class="sxs-lookup"><span data-stu-id="d97d0-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="d97d0-118">**1 ιουλίου 2020** Δεν μπορείτε πλέον να δημιουργείτε νέες αναζητήσεις και να διατηρείτε, αλλά μπορείτε να εκτελείτε, να επεξεργάζεστε και να διαγράφετε υπάρχουσες αναζητήσεις με δική σας ευθύνη.</span><span class="sxs-lookup"><span data-stu-id="d97d0-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="d97d0-119">Η υποστήριξη της Microsoft δεν υποστηρίζει πλέον την επιτόπια ανακάλυψη & διατηρεί στην ΑΗΚ.</span><span class="sxs-lookup"><span data-stu-id="d97d0-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="d97d0-120">**1 οκτωβρίου 2020** Η επιτόπια ανακάλυψη & διατηρεί τη λειτουργικότητα στην ΑΗΚ θα τοποθετηθεί σε λειτουργία μόνο για ανάγνωση, ώστε να μπορείτε να καταργήσετε μόνο τις υπάρχουσες αναζητήσεις και τις διαλαβές.</span><span class="sxs-lookup"><span data-stu-id="d97d0-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="d97d0-121">**Για περισσότερες πληροφορίες, ανατρέξτε στα**θέματα:</span><span class="sxs-lookup"><span data-stu-id="d97d0-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="d97d0-122">Μετεγκατάσταση αναζητήσεων ανακάλυψης παλαιού τύπου και συγκρατεί στο κέντρο συμμόρφωσης του Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="d97d0-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="d97d0-123">Συνταξιοδότηση των εργαλείων ανακάλυψης παλαιού τύπου</span><span class="sxs-lookup"><span data-stu-id="d97d0-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="d97d0-124">Συχνές ερωτήσεις σχετικά με την επιτόπια ανακάλυψη και την επιτόπια κατοχή</span><span class="sxs-lookup"><span data-stu-id="d97d0-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



