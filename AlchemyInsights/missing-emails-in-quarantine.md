---
title: Μηνύματα ηλεκτρονικού ταχυδρομείου που λείπουν σε καραντίνα
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 61a926c363c62bc7acb5efefe42b834f33c78eb6
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569229"
---
# <a name="missing-emails-in-quarantine"></a>Λείπουν μηνύματα ηλεκτρονικού ταχυδρομείου σε καραντίνα"

Οι διαχειριστές μπορούν να [προβάλλουν, να απελευθερώνουν ή να διαγράφουν αυτά τα μηνύματα.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Για να ανοίξετε το Κέντρο συμμόρφωσης & ασφαλείας, μεταβείτε στο [https://protection.office.com](https://protection.office.com/) . Για να ανοίξετε απευθείας τη σελίδα καραντίνας, μεταβείτε στο [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Μπορείτε να κάνετε αναζήτηση με τις ακόλουθες τιμές:  

- **Αναγνωριστικό μηνύματος**: Το καθολικά μοναδικό αναγνωριστικό του μηνύματος. Εάν επιλέξετε ένα μήνυμα στη λίστα, η τιμή **αναγνωριστικού μηνύματος** εμφανίζεται στο αναδυόμενο παράθυρο **Λεπτομερειών** που εμφανίζεται. Οι διαχειριστές μπορούν να χρησιμοποιήσουν [την ανίχνευση μηνυμάτων](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) για να εντοπίσουν μηνύματα και τις αντίστοιχες τιμές αναγνωριστικού μηνύματος.
- **Διεύθυνση ηλεκτρονικού ταχυδρομείου αποστολέα:** Η διεύθυνση ηλεκτρονικού ταχυδρομείου ενός μεμονωμένου αποστολέα.
- **Διεύθυνση ηλεκτρονικού ταχυδρομείου παραλήπτη**: Διεύθυνση ηλεκτρονικού ταχυδρομείου ενός παραλήπτη.
- **Θέμα:** Χρησιμοποιήστε ολόκληρο το θέμα του μηνύματος. Στην αναζήτηση δεν έγινε διάκριση πεζών-κεφαλαίων.

Αφού εισαγάγετε τα κριτήρια αναζήτησης, κάντε κλικ στο ![ κουμπί ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Ανανέωση** για να φιλτράρετε τα αποτελέσματα.  

Τα cmdlets που χρησιμοποιείτε για την προβολή και τη διαχείριση μηνυμάτων και αρχείων σε καραντίνα είναι τα:
- [Διαγραφή μηνύματος καραντίνας](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Εξαγωγή-καραντίνα Μήνυμα](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Μήνυμα "Get-Καραντίνα"](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Προεπισκόπηση-ΚαραντίναΜήνυμα:](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)Σημειώστε ότι αυτό το cmdlet προορίζεται μόνο για μηνύματα και όχι για αρχεία κακόβουλου λογισμικού από την ATP για το SharePoint Online, το OneDrive για επιχειρήσεις ή τις ομάδες.
- [Μήνυμα καραντίνας έκδοσης](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)