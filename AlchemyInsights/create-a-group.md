---
title: Δημιουργία ομάδας
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
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088904"
---
# <a name="create-a-group"></a>Δημιουργία ομάδας

Αυτό το θέμα περιγράφει τη δημιουργία ομάδας.

**Δικαίωμα δημιουργίας ομάδας**

Βεβαιωθείτε ότι είστε εξουσιοδοτημένοι να δημιουργήσετε μια νέα ομάδα. Οι Καθολικοί διαχειριστές μπορούν να απενεργοποιήσουν τη δημιουργία ομάδας στην πύλη Azure ή στον πίνακα πρόσβασης. Μπορεί να χρειαστείτε ένα διαχειριστή για να δημιουργήσετε τη νέα ομάδα για εσάς ή για να σας παρέχει τα κατάλληλα δικαιώματα.

**Διαχείριση δικαιωμάτων δημιουργίας ομάδας**

1. Οι Καθολικοί διαχειριστές μπορούν να διαχειριστούν τα δικαιώματα δημιουργίας ομάδας (για λόγους που σχετίζονται με την ασφάλεια) ή τις ομάδες του Office 365 που δημιουργήθηκαν στην πύλη Azure ή στον πίνακα Access, επιλέγοντας "οι χρήστες μπορούν να δημιουργήσουν ομάδες ασφαλείας σε θύρες Azure" ή "οι χρήστες μπορούν να δημιουργήσουν ομάδες του Office 365 σε Azure portals" επιλογές σε όλες τις γενικές **ομάδες**  >  **(ρυθμίσεις)**.
2. Μπορείτε επίσης να περιορίσετε τη δημιουργία ομάδας για να επιλέξετε μια ομάδα χρηστών, εάν έχετε μια άδεια χρήσης του Azure Active Directory P1 Premium.

**Απενεργοποίηση ειδοποίησης καλωσορίσματος για τα νέα μέλη της ομάδας του Office 365**

Η ειδοποίηση καλωσορίσματος που στάλθηκε στους χρήστες που προστίθενται στο Office 365 Groups μπορεί να απενεργοποιηθεί ορίζοντας το **UnifiedGroupWelcomeMessageEnabled** σε FALSE στο PowerShell. Μάθετε σχετικά με αυτήν τη ρύθμιση [εδώ](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).

