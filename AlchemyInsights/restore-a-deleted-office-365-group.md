---
title: Επαναφορά διαγραμμένης ομάδας Του Microsoft 365
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
ms.openlocfilehash: caa2c8987eecb89bac3469bf9471847858cab0ba
ms.sourcegitcommit: ec99a3a2e1e6a13d9a829d65ad1692a607dc3a17
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/06/2021
ms.locfileid: "51597443"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Επαναφορά διαγραμμένης ομάδας Του Microsoft 365

Μπορείτε να επαναφέρετε μια διαγραμμένη ομάδα του Microsoft 365 ή το Microsoft Teams εντός 30 ημερών από τη διαγραφή.

1. Μεταβείτε στο [κέντρο διαχείρισης του Microsoft 365 για να](https://aka.ms/RestoreDeletedGroup) συνδεθείτε και να παρατίθενται οι διαγραμμένες ομάδες και ομάδες.

    **Σημείωση:** Συνδεθείτε χρησιμοποιώντας το λογαριασμό που έχει εκχωρηθεί στο διαχειριστή του μισθωτή ή στο ρόλο διαχειριστή ομάδων.

1. Επιλέξτε τη διαγραμμένη ομάδα του Microsoft 365/Teams για επαναφορά και κάντε κλικ στην επιλογή **"Επαναφορά ομάδας".**

    Εάν δεν είναι δυνατή η επαναφορά της ομάδας λόγω μιας διεύθυνσης SMTP σε διένεξη, χρησιμοποιήστε την ακόλουθη εντολή για να βρείτε το αντικείμενο που προκαλεί διένεξη και να καταργήσετε τη διεύθυνση SMTP:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Σημείωση:** Σε ορισμένες περιπτώσεις, μπορεί να διαρκέσει έως και 24 ώρες για την επαναφορά της ομάδας και όλων των δεδομένων της.

    Για περισσότερες πληροφορίες ή για να μάθετε πώς μπορείτε να επαναφέρετε ομάδες χρησιμοποιώντας το PowerShell, ανατρέξτε στο θέμα [Επαναφορά διαγραμμένης ομάδας του Microsoft 365.](https://go.microsoft.com/fwlink/?linkid=867802)