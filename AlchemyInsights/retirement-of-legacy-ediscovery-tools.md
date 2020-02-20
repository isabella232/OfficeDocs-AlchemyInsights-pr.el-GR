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
# <a name="retirement-of-legacy-ediscovery-tools"></a>Συνταξιοδότηση των εργαλείων ανακάλυψης παλαιού τύπου

Ως αποτέλεσμα της νέας και βελτιωμένης λειτουργίας ανακάλυψης στο κέντρο συμμόρφωσης της Microsoft 365, τα ακόλουθα εργαλεία ανακάλυψης παλαιού τύπου και commandlets θα αποσυρθεί κατά τους επόμενους μήνες:

- [Επιτόπου ανακάλυψης](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) και [επιτόπου κατέχει](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) στο κέντρο διαχείρισης του Exchange.

- Το Exchange Online PowerShell cmdlets που υποστηρίζουν επιτόπου ανακάλυψης και επιτόπου κατέχει. (Αυτά τα cmdlets αναγνωρίζονται συλλογικά ως *-MailboxSearch cmdlets.) Αυτό περιλαμβάνει τα ακόλουθα cmdlets:

    - [ΝΕΟ-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Έναρξη-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Το cmdlet [γραμματοκιβώτιο αναζήτησης](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) στο Exchange Online PowerShell.
- Τις ακόλουθες λειτουργίες στο API των υπηρεσιών Web του Exchange:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Office 365 προηγμένη ανακάλυψη v 1.0](https://docs.microsoft.com/en-us/microsoft-365/compliance/office-365-advanced-ediscovery)

**Χρονοδιάγραμμα για τη συνταξιοδότηση**:
- 1 Απριλίου 2020: δεν θα μπορείτε να δημιουργήσετε νέες αναζητήσεις και να διατηρείτε, αλλά μπορείτε ακόμα να εκτελέσετε, να επεξεργαστείτε και να διαγράψετε υπάρχουσες αναζητήσεις με δική σας ευθύνη. Η υποστήριξη της Microsoft δεν θα υποστηρίζει πλέον επιτόπου ανακάλυψης & διατηρεί στην ΑΗΚ.

- 1 Ιουλίου 2020: η επιτόπου ανακάλυψης & κατέχει λειτουργικότητα στην ΑΗΚ θα τοποθετηθεί σε λειτουργία μόνο για ανάγνωση. Αυτό σημαίνει ότι θα είστε σε θέση να αφαιρέσετε μόνο τις υπάρχουσες αναζητήσεις και διατηρεί.

**Για περισσότερες πληροφορίες, ανατρέξτε**στο:

 - [Μετεγκατάσταση αναζητήσεις ανακάλυψης παλαιού τύπου και διατηρεί στο κέντρο συμμόρφωσης Microsoft 365](https://docs.microsoft.com/en-us/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Συνταξιοδότηση των εργαλείων ανακάλυψης παλαιού τύπου](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Συχνές ερωτήσεις σχετικά με την επιτόπου ανακάλυψη και επιτόπου κατέχει](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



