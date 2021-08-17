---
title: Μηνύματα ηλεκτρονικού ταχυδρομείου που λείπουν σε καραντίνα
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
- "5668"
- "9002625"
ms.openlocfilehash: bd5a04fd5abad962b4e85e009a9232e1a93219c238c629506df5cfb034453df2
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57892047"
---
# <a name="missing-emails-in-quarantine"></a>Μηνύματα ηλεκτρονικού ταχυδρομείου που λείπουν σε καραντίνα

Οι διαχειριστές μπορούν να [προβάλουν, να κυκλοφορούν ή να διαγράψουν αυτά τα μηνύματα](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

Στην πύλη Microsoft 365 Defender, μεταβείτε <https://security.microsoft.com> στην περιοχή "Αναθεώρηση  \> **καραντίνας".** Εναλλακτικά, για να μεταβείτε απευθείας στη **σελίδα "Καραντίνα",** χρησιμοποιήστε <https://security.microsoft.com/quarantine> το .  

Για περισσότερες πληροφορίες σχετικά με τις τιμές αναζήτησης/φίλτρου που μπορείτε να χρησιμοποιήσετε, ανατρέξτε στο θέμα Διαχείριση μηνυμάτων και αρχείων σε καραντίνα [ως διαχειριστής στο EOP.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

Τα cmdlet που χρησιμοποιείτε για να προβάλετε και να διαχειριστείτε μηνύματα και αρχεία σε καραντίνα είναι τα εξής:

- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage:](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)Σημειώστε ότι αυτό το cmdlet είναι μόνο για μηνύματα και όχι για αρχεία από Θυρίδα Συνημμένα για SharePoint, OneDrive ή Microsoft Teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)
