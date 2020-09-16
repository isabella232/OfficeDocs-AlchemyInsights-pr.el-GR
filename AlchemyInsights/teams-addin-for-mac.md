---
title: Πρόσθετο "ομάδες" για Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "9003233"
ms.openlocfilehash: 1e5f6d66386398ad8600f9383f9f7a1dcf0ce69f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670328"
---
# <a name="teams-add-in-for-mac"></a>Πρόσθετο "ομάδες" για Mac

Για να αντιμετωπίσετε ένα πρόσθετο που λείπει από τις ομάδες για τους χρήστες του λειτουργικού συστήματος για Mac, ακολουθήστε τα παρακάτω βήματα:

**Βήμα 1:** Εάν έχετε υβριδική Exchange εσωτερικής εγκατάστασης (2016 CU3 ή νεότερη έκδοση), χρησιμοποιήστε το εργαλείο Test-HMA.ps1 για να επιβεβαιώσετε ότι έχει ρυθμιστεί σωστά ο υβριδικός σύγχρονος έλεγχος ταυτότητας. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [επικύρωση υβριδικών σύγχρονων ρυθμίσεων ελέγχου ταυτότητας για το Outlook για iOS και Android](https://aka.ms/AA980zq).  

**Σημείωση** Χρήση της μορφής διεύθυνσης UPN (για παράδειγμα, [username@contoso.com](mailto:username@contoso.com)), όχι DOMAIN\username. Κάντε αυτό ακόμα και για τους χρήστες με γραμματοκιβώτια του Exchange Online.

**Βήμα 2:** Ζητήστε από το χρήστη να **Tools**μετακινήσει σε  >  **λογαριασμούς**εργαλείων... στο Outlook για Mac και εντοπίστε και επιλέξτε το λογαριασμό. Επιβεβαιώστε ότι το όνομα χρήστη που παρατίθεται είναι σε μορφή UPN (για παράδειγμα, [username@contoso.com](mailto:username@contoso.com)).

**Βήμα 3:** Επιβεβαιώστε ότι ο χρήστης είναι ένας χρήστης με άδεια χρήσης του Microsoft teams. Ο χρήστης πρέπει να χρησιμοποιεί τη συνδρομή του Office 365 για Mac, έκδοση προϊόντος 16,24 ή νεότερη.