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
ms.openlocfilehash: 2e7f898ac1a9e9469f633192be18e2a3a362023c83c9e510593196b5a4a0daf5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54074674"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Απόσυρση παλαιού τύπου εργαλείων eDiscovery

Ως αποτέλεσμα της νέας και βελτιωμένης λειτουργικότητας eDiscovery στο κέντρο συμμόρφωσης του Microsoft 365, τα ακόλουθα εργαλεία και τα commandlet eDiscovery παλαιού τύπου θα αποσυρθούν τους επόμενους μήνες:

- [In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.

- Τα Exchange Online cmdlet του PowerShell που υποστηρίζουν In-Place eDiscovery και In-Place χωρά. (Αυτά τα cmdlet αναγνωρίζονται συλλογικά ως cmdlet *-MailboxSearch.) Σε αυτά περιλαμβάνονται τα ακόλουθα cmdlet:

    - [Νέα-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Το [cmdlet γραμματοκιβωτίου](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) αναζήτησης στο Exchange Online PowerShell.
- Οι ακόλουθες λειτουργίες στο API Exchange Web Services:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Advanced eDiscovery v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Λωρίδα χρόνου απόσυρσης:**
- **1 Ιουλίου 2020** Δεν μπορείτε πλέον να δημιουργήσετε νέες αναζητήσεις και κάτοχους, αλλά μπορείτε να εκτελέσετε, να επεξεργαστείτε και να διαγράψετε υπάρχουσες αναζητήσεις με δική σας ευθύνη. Η Υποστήριξη της Microsoft δεν υποστηρίζει πλέον In-Place το eDiscovery & χωρά στο EAC.
    
- **1 Οκτωβρίου 2020** In-Place η λειτουργία "Κάτοχος" του eDiscovery & στο EAC θα τοποθετηθεί σε λειτουργία μόνο για ανάγνωση, ώστε να μπορείτε να καταργήσετε μόνο υπάρχουσες αναζητήσεις και κάτοχους.

**Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα:**

 - [Η μετεγκατάσταση παλαιού τύπου eDiscovery πραγματοποιεί αναζήτηση και χωρά στο Κέντρο συμμόρφωσης Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Απόσυρση παλαιού τύπου εργαλείων eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Συνήθεις ερωτήσεις σχετικά με In-Place eDiscovery και In-Place χωρά](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



