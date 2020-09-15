---
title: Ο συγχρονισμός της υπηρεσίας καταλόγου Active Directory δεν είναι
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3517f424b4dcd89f915acebab747a9bff993fdbd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47697629"
---
# <a name="active-directory-not-syncing"></a>Ο συγχρονισμός της υπηρεσίας καταλόγου Active Directory δεν είναι

Εάν λαμβάνετε σφάλματα συγχρονισμού, όπως "χωρίς πρόσφατο συγχρονισμό" ή Παρατηρήστε ότι η κατάσταση συγχρονισμού καταλόγου στην πύλη διαχείρισης του Office αναφέρει ότι "τελευταία συγχρονισμός πριν από περισσότερες από 3 ημέρες", μπορεί να είναι ότι το AADConnect έχει εσφαλμένες ρυθμίσεις ή ανεπαρκή δικαιώματα για την εκτέλεση συγχρονισμού.  

Η επανεγκατάσταση του AADConnect με τη χρήση των ρυθμίσεων Express μπορεί να επιλύσει το πρόβλημα γρήγορα:

1. [Πραγματοποιήστε λήψη της τελευταίας έκδοσης του AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [Ακολουθήστε τις οδηγίες για τη γρήγορη εγκατάσταση](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

Για περισσότερες πληροφορίες σχετικά με τους λογαριασμούς υπηρεσίας AADConnect, ανατρέξτε στο θέμα [σύνδεση του Azure AD: λογαριασμοί και δικαιώματα](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).
