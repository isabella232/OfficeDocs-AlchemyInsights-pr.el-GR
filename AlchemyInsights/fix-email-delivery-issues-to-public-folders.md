---
title: Επιδιορθώστε προβλήματα παράδοσης ηλεκτρονικού ταχυδρομείου για δημόσιους φακέλους με δυνατότητα αλληλογραφίας
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: e24a4db2deb3f691209a1634d932ed277a79c868
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35387705"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Επιδιορθώστε προβλήματα παράδοσης ηλεκτρονικού ταχυδρομείου για δημόσιους φακέλους με δυνατότητα αλληλογραφίας

Εάν εξωτερικοί αποστολείς δεν είναι δυνατό να στείλετε μηνύματα στους δημόσιους φακέλους σας με δυνατότητα αλληλογραφίας και τους αποστολείς να εμφανιστεί το μήνυμα λάθους: **δεν ήταν δυνατή η εύρεση (550 5.4.1)**, επιβεβαιώστε τον τομέα ηλεκτρονικού ταχυδρομείου για τον δημόσιο φάκελο που έχει ρυθμιστεί ως μια εσωτερική αναμετάδοσης τομέα αντί για ένα επιτακτική τομέα:

1. Ανοίξτε το [Κέντρο διαχείρισης Exchange (ΕΚΟ)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Μεταβείτε στην **ροή αλληλογραφίας** \> **δεκτά τομέων**, επιλέξτε τον τομέα που έγινε αποδεκτή και, στη συνέχεια, κάντε κλικ στο κουμπί **Επεξεργασία**.

3. Στις ιδιότητες σελίδας που ανοίγει, εάν έχει οριστεί ο τύπος τομέα **Authoritative**, αλλάξτε την τιμή σε **εσωτερικό αναμετάδοσης** και, στη συνέχεια, κάντε κλικ στο κουμπί **Αποθήκευση**.

Εάν εξωτερικοί αποστολείς, λαμβάνετε το σφάλμα που **δεν έχετε δικαίωμα (550 5.7.13)**, εκτελέστε την ακόλουθη εντολή στο [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) για να δείτε τα δικαιώματα για τους ανώνυμους χρήστες στο δημόσιο φάκελο:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Για παράδειγμα, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.

Για να επιτρέπεται στους εξωτερικούς χρήστες να στείλετε μήνυμα ηλεκτρονικού ταχυδρομείου σε αυτόν τον δημόσιο φάκελο, προσθέστε την πρόσβαση CreateItems δεξιά ο ανώνυμος χρήστης. Για παράδειγμα, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.
