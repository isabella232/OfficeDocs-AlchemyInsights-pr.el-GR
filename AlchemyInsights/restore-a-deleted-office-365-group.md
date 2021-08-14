---
title: Επαναφορά διαγραμμένης Microsoft 365 ομάδας
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: 6262ca04335c355fb4de41a9e1d854b666f47e10321a843717d6eb951c46cafd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53959026"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Επαναφορά διαγραμμένης Microsoft 365 ομάδας

Μπορείτε να επαναφέρετε μια διαγραμμένη Microsoft 365 ή Microsoft Teams εντός 30 ημερών από τη διαγραφή.

1. Μεταβείτε στην [Κέντρο διαχείρισης Microsoft 365](https://aka.ms/RestoreDeletedGroup) για να συνδεθείτε σε μια λίστα με τις ομάδες και τις ομάδες που έχετε διαγράψει.

    **Σημείωση:** Συνδεθείτε χρησιμοποιώντας το λογαριασμό που έχει εκχωρηθεί στο διαχειριστή του μισθωτή ή στο ρόλο διαχειριστή ομάδων.

1. Επιλέξτε τη διαγραμμένη Microsoft 365 ομάδας/Teams για επαναφορά και κάντε κλικ στην επιλογή **"Επαναφορά ομάδας".**

    Εάν δεν είναι δυνατή η επαναφορά της ομάδας λόγω μιας διεύθυνσης SMTP σε διένεξη, χρησιμοποιήστε την ακόλουθη εντολή για να βρείτε το αντικείμενο που προκαλεί διένεξη και να καταργήσετε τη διεύθυνση SMTP:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Σημείωση:** Σε ορισμένες περιπτώσεις, μπορεί να διαρκέσει έως και 24 ώρες για την επαναφορά της ομάδας και όλων των δεδομένων της.

    Για περισσότερες πληροφορίες ή για να μάθετε πώς μπορείτε να επαναφέρετε ομάδες χρησιμοποιώντας το PowerShell, ανατρέξτε στο θέμα [Επαναφορά διαγραμμένης Microsoft 365 ομάδας.](https://go.microsoft.com/fwlink/?linkid=867802)