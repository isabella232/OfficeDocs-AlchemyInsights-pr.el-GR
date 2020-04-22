---
title: Επιδιόρθωση ζητημάτων παράδοσης ηλεκτρονικού ταχυδρομείου σε δημόσιους φακέλους με δυνατότητα αλληλογραφίας
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: e261fe60843555fa45927b0a6b36e1ccf79fb028
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716352"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Επιδιόρθωση ζητημάτων παράδοσης ηλεκτρονικού ταχυδρομείου σε δημόσιους φακέλους με δυνατότητα αλληλογραφίας

Εάν οι εξωτερικοί αποστολείς δεν μπορούν να στείλουν μηνύματα στους δημόσιους φακέλους με δυνατότητα αλληλογραφίας και οι αποστολείς λάβουν το σφάλμα: **δεν ήταν δυνατή η εύρευσή τους (550 5.4.1)**, επαληθεύστε ότι ο τομέας ηλεκτρονικού ταχυδρομείου για τον δημόσιο φάκελο έχει ρυθμιστεί ως εσωτερικός τομέας αναμετάδοσης αντί για έναν έγκυρο τομέα:

1. Ανοίξτε το κέντρο διαχείρισης του [Exchange (ΑΗΚ)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Μεταβείτε στην ενότητα \> **Αποδεκτοί τομείς ροής** **αλληλογραφίας** , επιλέξτε τον αποδεκτό τομέα και, στη συνέχεια, κάντε κλικ στην επιλογή **Επεξεργασία**.

3. Στη σελίδα ιδιοτήτων που ανοίγει, εάν ο τύπος τομέα έχει οριστεί σε **"Επίσημο",** αλλάξτε την τιμή σε **Εσωτερική αναμετάδοση** και, στη συνέχεια, κάντε κλικ στο κουμπί **Αποθήκευση**.

Εάν οι εξωτερικοί αποστολείς λάβουν το σφάλμα **που δεν έχετε δικαιώματα (550 5.7.13)**, εκτελέστε την ακόλουθη εντολή στο [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) για να δείτε τα δικαιώματα για ανώνυμους χρήστες στον δημόσιο φάκελο:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Για παράδειγμα, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.

Για να επιτρέψετε σε εξωτερικούς χρήστες να στέλνουν μηνύματα ηλεκτρονικού ταχυδρομείου σε αυτόν τον δημόσιο φάκελο, προσθέστε το δικαίωμα πρόσβασης CreateItems στον ανώνυμο χρήστη. Για παράδειγμα, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.
