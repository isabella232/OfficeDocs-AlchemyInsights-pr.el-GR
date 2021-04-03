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
ms.openlocfilehash: 6f640093cd099f20d3a95eede5c141ad74838b0b
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505686"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Επαναφορά διαγραμμένης ομάδας Του Microsoft 365

Μπορείτε να επαναφέρετε μια διαγραμμένη ομάδα του Microsoft 365 ή το Microsoft Teams εντός 30 ημερών από τη διαγραφή.

1. Για να συνδεθείτε στο Κέντρο διαχείρισης του Microsoft 365 και να παρατίθενται οι διαγραμμένες ομάδες και ομάδες, μεταβείτε στο Κέντρο διαχείρισης Microsoft [365.](https://aka.ms/RestoreDeletedGroup)

    **Σημείωση:** Συνδεθείτε χρησιμοποιώντας το λογαριασμό που έχει εκχωρηθεί στο διαχειριστή του μισθωτή ή στο ρόλο διαχειριστή ομάδων.

1. Επιλέξτε τη διαγραμμένη ομάδα του Microsoft 365/Teams για επαναφορά και κάντε κλικ στην επιλογή **"Επαναφορά ομάδας".**

    Εάν δεν είναι δυνατή η επαναφορά της ομάδας λόγω μιας διεύθυνσης SMTP σε διένεξη, χρησιμοποιήστε την ακόλουθη εντολή για να βρείτε το αντικείμενο που προκαλεί διένεξη και να καταργήσετε τη διεύθυνση SMTP:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Σημείωση:** Σε ορισμένες περιπτώσεις, μπορεί να διαρκέσει έως και 24 ώρες για την επαναφορά της ομάδας και όλων των δεδομένων της.

    Για περισσότερες πληροφορίες ή για να μάθετε πώς μπορείτε να επαναφέρετε ομάδες χρησιμοποιώντας το PowerShell, ανατρέξτε στο θέμα [Επαναφορά διαγραμμένης ομάδας του Microsoft 365.](https://go.microsoft.com/fwlink/?linkid=867802)