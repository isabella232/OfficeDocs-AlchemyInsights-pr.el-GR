---
title: Επιδιόρθωση ζητημάτων παράδοσης ηλεκτρονικού ταχυδρομείου σε δημόσιους φακέλους με δυνατότητα αλληλογραφίας
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: da35ae4bd911fb75f23cc1c99aacbaa2392425dd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677928"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Επιδιόρθωση ζητημάτων παράδοσης ηλεκτρονικού ταχυδρομείου σε δημόσιους φακέλους με δυνατότητα αλληλογραφίας

Εάν οι εξωτερικοί αποστολείς δεν μπορούν να στείλουν μηνύματα στους δημόσιους φακέλους με δυνατότητα αλληλογραφίας και οι αποστολείς λαμβάνουν το σφάλμα: **δεν ήταν δυνατή η εύρεση (550 5.4.1)**, επιβεβαιώστε ότι ο τομέας ηλεκτρονικού ταχυδρομείου για τον δημόσιο φάκελο έχει ρυθμιστεί ως εσωτερικός τομέας αναμετάδοσης αντί για έναν επίσημο τομέα:

1. Ανοίξτε το [Κέντρο διαχείρισης του Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Μεταβείτε στις περιοχές με αποδοχή **ροής αλληλογραφίας** \> **Accepted domains**, επιλέξτε τον τομέα που αποδέχτηκε και, στη συνέχεια, κάντε κλικ στην επιλογή **Επεξεργασία**.

3. Στη σελίδα ιδιοτήτων που ανοίγει, εάν ο τύπος τομέα έχει την τιμή " **έγκυρη**", αλλάξτε την τιμή σε **εσωτερική αναμετάδοση** και, στη συνέχεια, κάντε κλικ στην επιλογή **Αποθήκευση**.

Εάν οι εξωτερικοί αποστολείς λάβουν το σφάλμα **που δεν έχετε δικαιώματα (550 5.7.13)**, εκτελέστε την ακόλουθη εντολή στο [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) για να δείτε τα δικαιώματα για ανώνυμους χρήστες στον δημόσιο φάκελο:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Για παράδειγμα, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .

Για να επιτρέψετε στους εξωτερικούς χρήστες να στέλνουν μηνύματα ηλεκτρονικού ταχυδρομείου σε αυτόν το δημόσιο φάκελο, προσθέστε το δικαίωμα πρόσβασης του CreateItems στο χρήστη ανώνυμο. Για παράδειγμα, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .
