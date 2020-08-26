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
# <a name="retirement-of-legacy-ediscovery-tools"></a>Συνταξιοδότηση των εργαλείων ανακάλυψης παλαιού τύπου

Ως αποτέλεσμα της νέας και βελτιωμένης λειτουργικότητας ανακάλυψης στο κέντρο συμμόρφωσης του Microsoft 365, τα παρακάτω εργαλεία ανακάλυψης παλαιού τύπου και τα commandlets θα αποσύρονται τους επόμενους μήνες:

- Επιτόπια [ανακάλυψη](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) και [επιτόπου κατοχή](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) στο κέντρο διαχείρισης του Exchange.

- Τα cmdlet του Exchange Online PowerShell που υποστηρίζουν την επιτόπια ανακάλυψη και την επιτόπια κατοχή. (Αυτά τα cmdlets προσδιορίζονται συλλογικά ως *-MailboxSearch cmdlets.) Αυτό περιλαμβάνει τα ακόλουθα cmdlet:

    - [New-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Έναρξη-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Ορίστε-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Το cmdlet του [γραμματοκιβωτίου αναζήτησης](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) στο Exchange Online PowerShell.
- Τις ακόλουθες λειτουργίες στο API των υπηρεσιών Web του Exchange:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Προηγμένη ηλεκτρονική ανακάλυψη v 1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Λωρίδα χρόνου για συνταξιοδότηση**:
- **1 ιουλίου 2020** Δεν μπορείτε πλέον να δημιουργείτε νέες αναζητήσεις και να διατηρείτε, αλλά μπορείτε να εκτελείτε, να επεξεργάζεστε και να διαγράφετε υπάρχουσες αναζητήσεις με δική σας ευθύνη. Η υποστήριξη της Microsoft δεν υποστηρίζει πλέον την επιτόπια ανακάλυψη & διατηρεί στην ΑΗΚ.
    
- **1 οκτωβρίου 2020** Η επιτόπια ανακάλυψη & διατηρεί τη λειτουργικότητα στην ΑΗΚ θα τοποθετηθεί σε λειτουργία μόνο για ανάγνωση, ώστε να μπορείτε να καταργήσετε μόνο τις υπάρχουσες αναζητήσεις και τις διαλαβές.

**Για περισσότερες πληροφορίες, ανατρέξτε στα**θέματα:

 - [Μετεγκατάσταση αναζητήσεων ανακάλυψης παλαιού τύπου και συγκρατεί στο κέντρο συμμόρφωσης του Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Συνταξιοδότηση των εργαλείων ανακάλυψης παλαιού τύπου](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Συχνές ερωτήσεις σχετικά με την επιτόπια ανακάλυψη και την επιτόπια κατοχή](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



