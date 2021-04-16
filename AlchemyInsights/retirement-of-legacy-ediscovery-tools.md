---
title: Απόσυρση παλαιού τύπου εργαλείων eDiscovery
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 986c78f20e7b8c303c302913d63d817a56ce2896
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51798549"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="9b75a-102">Απόσυρση παλαιού τύπου εργαλείων eDiscovery</span><span class="sxs-lookup"><span data-stu-id="9b75a-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="9b75a-103">Ως αποτέλεσμα της νέας και βελτιωμένης λειτουργικότητας eDiscovery στο Κέντρο συμμόρφωσης του Microsoft 365, τα ακόλουθα εργαλεία και commandlet eDiscovery παλαιού τύπου θα αποσυρθούν τους επόμενους μήνες:</span><span class="sxs-lookup"><span data-stu-id="9b75a-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="9b75a-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span><span class="sxs-lookup"><span data-stu-id="9b75a-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="9b75a-105">Τα cmdlet του Exchange Online PowerShell που υποστηρίζουν In-Place eDiscovery και In-Place χωρά.</span><span class="sxs-lookup"><span data-stu-id="9b75a-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="9b75a-106">(Αυτά τα cmdlet αναγνωρίζονται συλλογικά ως cmdlet \*-MailboxSearch.) Σε αυτά περιλαμβάνονται τα ακόλουθα cmdlet:</span><span class="sxs-lookup"><span data-stu-id="9b75a-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="9b75a-107">Νέα-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="9b75a-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="9b75a-108">Start-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="9b75a-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="9b75a-109">Stop-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="9b75a-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="9b75a-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="9b75a-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="9b75a-111">Το [cmdlet γραμματοκιβωτίου](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) αναζήτησης στο Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="9b75a-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="9b75a-112">Οι ακόλουθες λειτουργίες στο API των υπηρεσιών Web Exchange:</span><span class="sxs-lookup"><span data-stu-id="9b75a-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="9b75a-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="9b75a-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="9b75a-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="9b75a-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="9b75a-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="9b75a-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="9b75a-116">Advanced eDiscovery v1.0</span><span class="sxs-lookup"><span data-stu-id="9b75a-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="9b75a-117">**Λωρίδα χρόνου απόσυρσης:**</span><span class="sxs-lookup"><span data-stu-id="9b75a-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="9b75a-118">**1 Ιουλίου 2020** Δεν μπορείτε πλέον να δημιουργήσετε νέες αναζητήσεις και κάτοχους, αλλά μπορείτε να εκτελέσετε, να επεξεργαστείτε και να διαγράψετε υπάρχουσες αναζητήσεις με δική σας ευθύνη.</span><span class="sxs-lookup"><span data-stu-id="9b75a-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="9b75a-119">Η Υποστήριξη της Microsoft δεν υποστηρίζει πλέον In-Place το eDiscovery & χωρά στο EAC.</span><span class="sxs-lookup"><span data-stu-id="9b75a-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="9b75a-120">**1 Οκτωβρίου 2020** In-Place η λειτουργία "Κάτοχος" του eDiscovery & στο EAC θα τοποθετηθεί σε λειτουργία μόνο για ανάγνωση, ώστε να μπορείτε να καταργήσετε μόνο υπάρχουσες αναζητήσεις και κάτοχους.</span><span class="sxs-lookup"><span data-stu-id="9b75a-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="9b75a-121">**Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα:**</span><span class="sxs-lookup"><span data-stu-id="9b75a-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="9b75a-122">Η μετεγκατάσταση παλαιού τύπου eDiscovery πραγματοποιεί αναζήτηση και μεταφορά στο κέντρο συμμόρφωσης του Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="9b75a-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="9b75a-123">Απόσυρση παλαιού τύπου εργαλείων eDiscovery</span><span class="sxs-lookup"><span data-stu-id="9b75a-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="9b75a-124">Συνήθεις ερωτήσεις σχετικά με In-Place eDiscovery και In-Place χωρά</span><span class="sxs-lookup"><span data-stu-id="9b75a-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



