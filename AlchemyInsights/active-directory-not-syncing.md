---
title: Η υπηρεσία καταλόγου Active Directory δεν συγχρονίζεται
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
- "9001688"
- "3754"
ms.openlocfilehash: 274855457a143cfccd25f9a161ff894882cee9c4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822851"
---
# <a name="active-directory-not-syncing"></a>Η υπηρεσία καταλόγου Active Directory δεν συγχρονίζεται

Εάν λαμβάνετε σφάλματα συγχρονισμού, όπως "δεν υπάρχει πρόσφατος συγχρονισμός" ή παρατηρήσετε ότι η κατάσταση συγχρονισμού καταλόγου στην πύλη διαχείρισης του Office αναφέρει "Ο τελευταίος συγχρονισμός έγινε πριν από περισσότερες από 3 ημέρες", μπορεί να είναι ότι το AADConnect έχει εσφαλμένες ρυθμίσεις ή ανεπαρκή δικαιώματα για την εκτέλεση συγχρονισμού.  

Η επανεγκατάσταση του AADConnect με τη χρήση των express ρυθμίσεων μπορεί να επιλύσει το πρόβλημα γρήγορα:

1. [Κάντε λήψη της πιο πρόσφατης έκδοσης του AADConnect.](https://go.microsoft.com/fwlink/?LinkId=615771)

2. [Ακολουθήστε τις οδηγίες για τη γρήγορη εγκατάσταση.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)

Για περισσότερες πληροφορίες σχετικά με τους λογαριασμούς υπηρεσιών AADConnect, ανατρέξτε στο [θέμα Azure AD Connect: Λογαριασμοί και δικαιώματα.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)
