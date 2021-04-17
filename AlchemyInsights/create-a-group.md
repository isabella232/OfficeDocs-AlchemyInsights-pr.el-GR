---
title: Δημιουργία ομάδας
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
- "9003234"
- "7230"
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816356"
---
# <a name="create-a-group"></a>Δημιουργία ομάδας

Αυτό το θέμα περιγράφει τη δημιουργία ομάδας.

**Δικαίωμα δημιουργίας ομάδας**

Βεβαιωθείτε ότι έχετε την εξουσιοδότηση να δημιουργήσετε μια νέα ομάδα. Οι καθολικοί διαχειριστές μπορούν να απενεργοποιήσουν τη δημιουργία ομάδας στην πύλη Azure ή στον Πίνακα πρόσβασης. Μπορεί να χρειαστείτε ένα διαχειριστή για να δημιουργήσετε τη νέα ομάδα για εσάς ή για να σας δώσει τα κατάλληλα δικαιώματα.

**Διαχείριση δικαιωμάτων δημιουργίας ομάδας**

1. Οι καθολικοί διαχειριστές μπορούν να διαχειρίζονται δικαιώματα δημιουργίας ομάδων (για λόγους ασφαλείας) ή ομάδες του Office 365 που έχουν δημιουργηθεί στην πύλη Azure ή στον Πίνακα πρόσβασης, επιλέγοντας "Οι χρήστες μπορούν να δημιουργούν ομάδες ασφαλείας σε πύλες Azure" ή "Οι χρήστες μπορούν να δημιουργήσουν ομάδες του Office 365 σε πύλες Azure" στις επιλογές "Γενικά  >  **(Ρυθμίσεις)** όλων των ομάδων.
2. Μπορείτε επίσης να περιορίσετε τη δημιουργία ομάδας για να επιλέξετε μια ομάδα χρηστών, εάν έχετε μια άδεια χρήσης Azure Active Directory P1 Premium.

**Απενεργοποίηση ειδοποίησης υποδοχής για νέα μέλη ομάδας του Office 365**

Η ειδοποίηση υποδοχής που αποστέλλεται στους χρήστες που προστίθενται σε ομάδες του Office 365 μπορεί να απενεργοποιηθεί, ορίζοντας το **UnifiedGroupWelcomeMessageEnabled** σε False στο Powershell. Μάθετε περισσότερα σχετικά με αυτήν τη [ρύθμιση εδώ.](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)

