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
ms.openlocfilehash: 563f76f624f428a46894268b478cf05eb757b497
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539824"
---
# <a name="missing-emails-in-quarantine"></a>Μηνύματα ηλεκτρονικού ταχυδρομείου που λείπουν σε καραντίνα"

Οι διαχειριστές μπορούν να [προβάλουν, να κυκλοφορούν ή να διαγράψουν αυτά τα μηνύματα.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

Για να ανοίξετε το Κέντρο & ασφαλείας, μεταβείτε στο [https://protection.office.com](https://protection.office.com/) . Για να ανοίξετε απευθείας τη σελίδα καραντίνας, μεταβείτε στην περιοχή [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Μπορείτε να κάνετε αναζήτηση με τις ακόλουθες τιμές:  

- **Αναγνωριστικό μηνύματος:** Το καθολικά μοναδικό αναγνωριστικό του μηνύματος. Εάν επιλέξετε ένα μήνυμα στη λίστα, η τιμή αναγνωριστικού  **μηνύματος**  εμφανίζεται στο αναδυόμενο  **παράθυρο**  λεπτομερειών που εμφανίζεται. Οι διαχειριστές μπορούν να χρησιμοποιήσουν [την ανίχνευση μηνύματος](/microsoft-365/security/office-365-security/message-trace-scc) για να εντοπίσουν τα μηνύματα και τις αντίστοιχες τιμές αναγνωριστικού μηνύματος.
- **Διεύθυνση ηλεκτρονικού ταχυδρομείου αποστολέα:** Η διεύθυνση ηλεκτρονικού ταχυδρομείου ενός αποστολέα.
- **Διεύθυνση ηλεκτρονικού ταχυδρομείου παραλήπτη:** Η διεύθυνση ηλεκτρονικού ταχυδρομείου ενός παραλήπτη.
- **Θέμα:** Χρησιμοποιήστε ολόκληρο το θέμα του μηνύματος. Η αναζήτηση δεν κάνει διάκριση πεζών-κεφαλαίων.

Αφού εισάγετε τα κριτήρια αναζήτησης, κάντε κλικ στο κουμπί ![ "Ανανέωση" ](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **ανανέωσης για** να φιλτράρετε τα αποτελέσματα.

Τα cmdlet που χρησιμοποιείτε για να προβάλετε και να διαχειριστείτε μηνύματα και αρχεία σε καραντίνα είναι τα εξής:
- [Delete-QuarantineMessage](/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage:](/powershell/module/exchange/preview-quarantinemessage)Σημειώστε ότι αυτό το cmdlet αφορά μόνο μηνύματα και όχι αρχεία κακόβουλης λειτουργίας από το Microsoft Defender για Office 365 για SharePoint Online, OneDrive για επιχειρήσεις ή Teams.
- [Release-QuarantineMessage](/powershell/module/exchange/release-quarantinemessage)