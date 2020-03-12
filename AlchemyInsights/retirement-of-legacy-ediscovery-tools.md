---
title: Συνταξιοδότηση εργαλείων eDiscovery παλαιού τύπου
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
ms.openlocfilehash: af9a0bd8ff4294575ac68f37d4997bb50b132ce7
ms.sourcegitcommit: 9ab422063e5a474c92ed956d42d222b90336fecb
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/11/2020
ms.locfileid: "42600369"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="82662-102">Συνταξιοδότηση εργαλείων eDiscovery παλαιού τύπου</span><span class="sxs-lookup"><span data-stu-id="82662-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="82662-103">Ως αποτέλεσμα της νέας και βελτιωμένης λειτουργικότητας eDiscovery στο Κέντρο συμμόρφωσης του Microsoft 365, τα ακόλουθα εργαλεία και κοέτες eDiscovery παλαιού τύπου θα αποσυρθούν τους επόμενους μήνες:</span><span class="sxs-lookup"><span data-stu-id="82662-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="82662-104">[Το in-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) και [το In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) στο κέντρο διαχείρισης του Exchange.</span><span class="sxs-lookup"><span data-stu-id="82662-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="82662-105">Τα cmdlets PowerShell του Exchange Online που υποστηρίζουν επιτόπια eDiscovery και in-place hold.</span><span class="sxs-lookup"><span data-stu-id="82662-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="82662-106">(Αυτά τα cmdlets αναγνωρίζονται συλλογικά ως \*-MailboxSearch cmdlets.) Αυτό περιλαμβάνει τα ακόλουθα cmdlets:</span><span class="sxs-lookup"><span data-stu-id="82662-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="82662-107">Αναζήτηση νέου γραμματοκιβωτίου</span><span class="sxs-lookup"><span data-stu-id="82662-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="82662-108">Αναζήτηση γραμματοκιβωτίου έναρξης</span><span class="sxs-lookup"><span data-stu-id="82662-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="82662-109">Αναζήτηση γραμματοκιβωτίου διακοπής</span><span class="sxs-lookup"><span data-stu-id="82662-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="82662-110">Αναζήτηση προκαθορισμένου γραμματοκιβωτίου</span><span class="sxs-lookup"><span data-stu-id="82662-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="82662-111">Το cmdlet [γραμματοκιβωτίου αναζήτησης](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) στο Ηλεκτρονικό PowerShell του Exchange.</span><span class="sxs-lookup"><span data-stu-id="82662-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="82662-112">Οι ακόλουθες λειτουργίες στο API των υπηρεσιών Web του Exchange:</span><span class="sxs-lookup"><span data-stu-id="82662-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="82662-113">Γραμματοκιβώτια με δυνατότητα αναζήτησης</span><span class="sxs-lookup"><span data-stu-id="82662-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="82662-114">Προκαθορισμένα γραμματοκιβώτια HoldOn</span><span class="sxs-lookup"><span data-stu-id="82662-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="82662-115">Κουτ-ντοκους</span><span class="sxs-lookup"><span data-stu-id="82662-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="82662-116">Office 365 για προχωρημένους eDiscovery v1.0</span><span class="sxs-lookup"><span data-stu-id="82662-116">Office 365 Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="82662-117">**Χρονοδιάγραμμα για τη συνταξιοδότηση:**</span><span class="sxs-lookup"><span data-stu-id="82662-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="82662-118">1 Απριλίου 2020: Δεν θα μπορείτε να δημιουργήσετε νέες αναζητήσεις και κρατήσεις, αλλά μπορείτε να εκτελέσετε, να επεξεργαστείτε και να διαγράψετε υπάρχουσες αναζητήσεις με δική σας ευθύνη.</span><span class="sxs-lookup"><span data-stu-id="82662-118">April 1, 2020: You won't be able to create new searches and holds, but you can still run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="82662-119">Η υποστήριξη της Microsoft δεν θα υποστηρίζει πλέον επιτόπιες & διατηρήσεις στην ΑΗΚ.</span><span class="sxs-lookup"><span data-stu-id="82662-119">Microsoft Support will no longer support In-Place eDiscovery & Holds in the EAC.</span></span>

- <span data-ttu-id="82662-120">1 Ιουλίου 2020: Η λειτουργία In-Place eDiscovery & Holds στην ΑΗΚ θα τοποθετηθεί σε λειτουργία μόνο για ανάγνωση.</span><span class="sxs-lookup"><span data-stu-id="82662-120">July 1, 2020: The In-Place eDiscovery & Holds functionality in the EAC will be placed in a read-only mode.</span></span> <span data-ttu-id="82662-121">Αυτό σημαίνει ότι θα μπορείτε να καταργήσετε μόνο υπάρχουσες αναζητήσεις και κρατήσεις.</span><span class="sxs-lookup"><span data-stu-id="82662-121">This means you'll only be able to remove existing searches and holds.</span></span>

<span data-ttu-id="82662-122">**Για περισσότερες πληροφορίες, ανατρέξτε στα θέματα**:</span><span class="sxs-lookup"><span data-stu-id="82662-122">**For more information, see**:</span></span>

 - [<span data-ttu-id="82662-123">Μετεγκατάσταση αναζητήσεων eDiscovery παλαιού τύπου και διατηρείται στο κέντρο συμμόρφωσης του Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="82662-123">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="82662-124">Συνταξιοδότηση εργαλείων eDiscovery παλαιού τύπου</span><span class="sxs-lookup"><span data-stu-id="82662-124">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="82662-125">Συνήθεις ερωτήσεις σχετικά με τις επιτόπιες βάσεις eDiscovery και in-place hold</span><span class="sxs-lookup"><span data-stu-id="82662-125">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



