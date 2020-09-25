---
title: εργαλείο εξαγωγής ανακάλυψης
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
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: 67e59182a5053111a08f5fb2be814931a1aa815d
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277937"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Δεν μπορείτε να εγκαταστήσετε ή να εκτελέσετε το εργαλείο εξαγωγής ανακάλυψης;

Εάν δεν μπορείτε να εγκαταστήσετε ή να εκτελέσετε το εργαλείο εξαγωγής ανακάλυψης για να κάνετε λήψη των αποτελεσμάτων αναζήτησης, ανατρέξτε στα παρακάτω στοιχεία:
  
- Ο υπολογιστής που χρησιμοποιείτε πληροί αυτές τις προϋποθέσεις:

  - εκδόσεις 32 ή 64-bit των Windows 7 και των νεότερων εκδόσεων

  - Microsoft .NET Framework 4.7

  - Ένα υποστηριζόμενο πρόγραμμα περιήγησης:

  - Microsoft Edge

    Ή

  - Internet Explorer 10 και νεότερες εκδόσεις

    Άλλα προγράμματα περιήγησης, όπως το Google Chrome και το Mozilla Firefox δεν υποστηρίζονται.

- Ο οργανισμός σας μπορεί να συνδεθεί με το τελικό σημείο στο Azure, το οποίο είναι ** \* . blob.Core.Windows.NET** (ο χαρακτήρας μπαλαντέρ αντιπροσωπεύει ένα μοναδικό αναγνωριστικό για την εργασία εξαγωγής).

- Σας έχει εκχωρηθεί ο ρόλος εξαγωγής στο κέντρο συμμόρφωσης ασφαλείας του Microsoft 365 &amp; . Από προεπιλογή, αυτός ο ρόλος εκχωρείται μόνο στην ομάδα ρόλων της διαχείρισης ανακάλυψης. Ανατρέξτε στο θέμα [εκχώρηση δικαιωμάτων ανακάλυψης](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).

Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Εξαγωγή αποτελεσμάτων αναζήτησης περιεχομένου](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).

Εάν εξάγετε περισσότερα από 100K γραμματοκιβώτια, θα πρέπει να χρησιμοποιήσετε το ακόλουθο PowerShell για να κάνετε λήψη των αποτελεσμάτων εξαγωγής:  [Εξαγωγή αποτελεσμάτων από περισσότερα από 100K γραμματοκιβώτια](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).