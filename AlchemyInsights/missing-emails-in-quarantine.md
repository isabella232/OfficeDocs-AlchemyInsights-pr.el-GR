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
ms.openlocfilehash: 43f9a1f03084bf9adab706b3f77eff1d1db888ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831734"
---
# <a name="missing-emails-in-quarantine"></a>Μηνύματα ηλεκτρονικού ταχυδρομείου που λείπουν σε καραντίνα"

Οι διαχειριστές μπορούν να [προβάλουν, να κυκλοφορούν ή να διαγράψουν αυτά τα μηνύματα.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Για να ανοίξετε το Κέντρο & ασφαλείας, μεταβείτε στο [https://protection.office.com](https://protection.office.com/) . Για να ανοίξετε απευθείας τη σελίδα καραντίνας, μεταβείτε στην περιοχή [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Μπορείτε να κάνετε αναζήτηση με τις ακόλουθες τιμές:  

- **Αναγνωριστικό μηνύματος:** Το καθολικά μοναδικό αναγνωριστικό του μηνύματος. Εάν επιλέξετε ένα μήνυμα στη λίστα, η τιμή αναγνωριστικού  **μηνύματος**  εμφανίζεται στο αναδυόμενο  **παράθυρο**  λεπτομερειών που εμφανίζεται. Οι διαχειριστές μπορούν να χρησιμοποιήσουν [την ανίχνευση μηνύματος](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) για να εντοπίσουν τα μηνύματα και τις αντίστοιχες τιμές αναγνωριστικού μηνύματος.
- **Διεύθυνση ηλεκτρονικού ταχυδρομείου αποστολέα:** Η διεύθυνση ηλεκτρονικού ταχυδρομείου ενός αποστολέα.
- **Διεύθυνση ηλεκτρονικού ταχυδρομείου παραλήπτη:** Η διεύθυνση ηλεκτρονικού ταχυδρομείου ενός παραλήπτη.
- **Θέμα:** Χρησιμοποιήστε ολόκληρο το θέμα του μηνύματος. Η αναζήτηση δεν κάνει διάκριση πεζών-κεφαλαίων.

Αφού εισάγετε τα κριτήρια αναζήτησης, κάντε κλικ στο κουμπί ![ "Ανανέωση" ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **ανανέωσης για** να φιλτράρετε τα αποτελέσματα.  

Τα cmdlet που χρησιμοποιείτε για να προβάλετε και να διαχειριστείτε μηνύματα και αρχεία σε καραντίνα είναι τα εξής:
- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage:](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)Σημειώστε ότι αυτό το cmdlet αφορά μόνο τα μηνύματα και όχι τα αρχεία κακόβουλου λογισμικού από atp για το SharePoint Online, το OneDrive για επιχειρήσεις ή το Teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)