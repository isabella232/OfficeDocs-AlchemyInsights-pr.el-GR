---
title: Η υπηρεσία καταλόγου Active Directory δεν συγχρονίζεται
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3abad160ab28922685d235a1fa546105e31757fb
ms.sourcegitcommit: d87a6ac6ee77375d1d750100359b4dc7b2871691
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 02/25/2020
ms.locfileid: "42265196"
---
# <a name="active-directory-not-syncing"></a>Η υπηρεσία καταλόγου Active Directory δεν συγχρονίζεται

Εάν λαμβάνετε σφάλματα συγχρονισμού, όπως "χωρίς πρόσφατο συγχρονισμό" ή παρατηρήσετε την κατάσταση συγχρονισμού καταλόγου στην πύλη διαχείρισης του Office λέει, "τελευταία συγχρονισμός περισσότερο από 3 ημέρες πριν," μπορεί να είναι ότι AADConnect έχει εσφαλμένες ρυθμίσεις ή ανεπαρκής δικαιώματα για την εκτέλεση συγχρονισμού.  

Η επανεγκατάσταση του AADConnect χρησιμοποιώντας τις γρήγορες ρυθμίσεις ενδέχεται να επιλύσει το ζήτημα γρήγορα:

1. [Κατεβάστε την τελευταία έκδοση του AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [Ακολουθήστε τις οδηγίες για τη γρήγορη εγκατάσταση](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

Για περισσότερες πληροφορίες σχετικά με τους λογαριασμούς υπηρεσίας AADConnect, ανατρέξτε στο θέμα [σύνδεση AD Azure: λογαριασμοί και δικαιώματα](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).
