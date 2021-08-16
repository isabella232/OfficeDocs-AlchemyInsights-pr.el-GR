---
title: Εργαλείο εξαγωγής eDiscovery
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
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: f7b7e1ae4f1f686fa510403d398c4ff750dbadb9065b8d63701a927eeac52d9b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101302"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Δεν μπορείτε να εγκαταστήσετε ή να εκτελέσετε το Εργαλείο εξαγωγής eDiscovery;

Εάν δεν μπορείτε να εγκαταστήσετε ή να εκτελέσετε το Εργαλείο εξαγωγής eDiscovery για να κάνετε λήψη των αποτελεσμάτων αναζήτησης, ελέγξτε τα εξής:
  
- Ο υπολογιστής που χρησιμοποιείτε πληροί τα εξής προαπαιτούμενα:

  - Εκδόσεις 32 ή 64 bit του Windows 7 και νεότερες εκδόσεις

  - Microsoft .NET Framework 4.7

  - Ένα υποστηριζόμενο πρόγραμμα περιήγησης:

  - Microsoft Edge

    Ή

  - Internet Explorer 10 και νεότερες εκδόσεις

    Άλλα προγράμματα περιήγησης, όπως το Google Chrome και το Mozilla Firefox δεν υποστηρίζονται.

- Ο οργανισμός σας μπορεί να συνδεθεί με το τελικό σημείο στο Azure, το οποίο είναι **\* .blob.core.windows.net** (ο χαρακτήρες μπαλαντέρ αντιπροσωπεύει ένα μοναδικό αναγνωριστικό για την εργασία εξαγωγής).

- Σας έχει εκχωρηθεί ο ρόλος "Εξαγωγή" στο κέντρο Microsoft 365 &amp; συμμόρφωσης ασφαλείας. Από προεπιλογή, αυτός ο ρόλος εκχωρείται μόνο στην ομάδα ρόλων της Διαχείρισης eDiscovery. Ανατρέξτε [στο θέμα Εκχώρηση δικαιωμάτων eDiscovery.](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions)

Για περισσότερες πληροφορίες, ανατρέξτε στο [θέμα "Εξαγωγή αποτελεσμάτων αναζήτησης περιεχομένου".](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)

Εάν εξάγετε περισσότερα από 100K γραμματοκιβώτια, θα πρέπει να χρησιμοποιήσετε το ακόλουθο Powershell για να κάνετε λήψη των αποτελεσμάτων εξαγωγής: Εξαγωγή αποτελεσμάτων από περισσότερα από [100K γραμματοκιβώτια.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)