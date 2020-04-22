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
ms.openlocfilehash: 262cca0feee17d1f929a5a94a4dd6c1ec317f6ec
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/21/2020
ms.locfileid: "43650568"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Συνταξιοδότηση εργαλείων eDiscovery παλαιού τύπου

Ως αποτέλεσμα της νέας και βελτιωμένης λειτουργικότητας eDiscovery στο Κέντρο συμμόρφωσης του Microsoft 365, τα ακόλουθα εργαλεία και κοέτες eDiscovery παλαιού τύπου θα αποσυρθούν τους επόμενους μήνες:

- [Το in-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) και [το In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) στο κέντρο διαχείρισης του Exchange.

- Τα cmdlets PowerShell του Exchange Online που υποστηρίζουν επιτόπια eDiscovery και in-place hold. (Αυτά τα cmdlets αναγνωρίζονται συλλογικά ως *-MailboxSearch cmdlets.) Αυτό περιλαμβάνει τα ακόλουθα cmdlets:

    - [Αναζήτηση νέου γραμματοκιβωτίου](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Αναζήτηση γραμματοκιβωτίου έναρξης](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Αναζήτηση γραμματοκιβωτίου διακοπής](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Αναζήτηση προκαθορισμένου γραμματοκιβωτίου](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Το cmdlet [γραμματοκιβωτίου αναζήτησης](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) στο Ηλεκτρονικό PowerShell του Exchange.
- Οι ακόλουθες λειτουργίες στο API των υπηρεσιών Web του Exchange:
    - [Γραμματοκιβώτια με δυνατότητα αναζήτησης](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [Προκαθορισμένα γραμματοκιβώτια HoldOn](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [Κουτ-ντοκους](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Προηγμένο eDiscovery v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Χρονοδιάγραμμα για τη συνταξιοδότηση:**
- 1 Απριλίου 2020: Δεν θα μπορείτε να δημιουργήσετε νέες αναζητήσεις και κρατήσεις, αλλά μπορείτε να εκτελέσετε, να επεξεργαστείτε και να διαγράψετε υπάρχουσες αναζητήσεις με δική σας ευθύνη. Η υποστήριξη της Microsoft δεν θα υποστηρίζει πλέον επιτόπιες & διατηρήσεις στην ΑΗΚ.

- 1 Ιουλίου 2020: Η λειτουργία In-Place eDiscovery & Holds στην ΑΗΚ θα τοποθετηθεί σε λειτουργία μόνο για ανάγνωση. Αυτό σημαίνει ότι θα μπορείτε να καταργήσετε μόνο υπάρχουσες αναζητήσεις και κρατήσεις.

**Για περισσότερες πληροφορίες, ανατρέξτε στα θέματα**:

 - [Μετεγκατάσταση αναζητήσεων eDiscovery παλαιού τύπου και διατηρείται στο κέντρο συμμόρφωσης του Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Συνταξιοδότηση εργαλείων eDiscovery παλαιού τύπου](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Συνήθεις ερωτήσεις σχετικά με τις επιτόπιες βάσεις eDiscovery και in-place hold](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



