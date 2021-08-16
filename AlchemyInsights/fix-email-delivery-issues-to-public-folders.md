---
title: Επιδιόρθωση προβλημάτων παράδοσης ηλεκτρονικού ταχυδρομείου σε δημόσιους φακέλους με δυνατότητα αλληλογραφίας
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
ms.openlocfilehash: ff1400f694ae037a8658356af068b4c20b8fa9d9908dafedb90db7bb6859530f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068812"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Επιδιόρθωση προβλημάτων παράδοσης ηλεκτρονικού ταχυδρομείου σε δημόσιους φακέλους με δυνατότητα αλληλογραφίας

Εάν οι εξωτερικοί αποστολείς δεν μπορούν να στείλουν μηνύματα σε δημόσιους φακέλους με δυνατότητα αλληλογραφίας και οι αποστολείς λάβουν το σφάλμα: δεν ήταν δυνατός ο βρείτε **(550 5.4.1),** επαληθεύστε ότι ο τομέας ηλεκτρονικού ταχυδρομείου για τον δημόσιο φάκελο έχει ρυθμιστεί ως τομέας εσωτερικής αναμετάδοσης αντί για έναν επίσημο τομέα:

1. Ανοίξτε το [Exchange διαχείρισης (EAC).](https://docs.microsoft.com/Exchange/exchange-admin-center)

2. Μεταβείτε στην **περιοχή "Αποδεκτοί** \> **τομείς ροής αλληλογραφίας",** επιλέξτε τον αποδεκτό τομέα και, στη συνέχεια, κάντε κλικ στην επιλογή **"Επεξεργασία".**

3. Στη σελίδα ιδιοτήτων που ανοίγει, εάν ο τύπος τομέα έχει οριστεί σε "Έγκυρα", αλλάξτε την τιμή σε "Εσωτερική αναμετάδοση" και, στη **συνέχεια,** κάντε κλικ στην επιλογή **"Αποθήκευση".** 

Εάν οι εξωτερικοί αποστολείς λάβουν το σφάλμα που δεν έχετε δικαιώματα **(550 5.7.13),** εκτελέστε την ακόλουθη εντολή στο [Exchange Online PowerShell για να](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) δείτε τα δικαιώματα για ανώνυμους χρήστες στον δημόσιο φάκελο:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Για παράδειγμα, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .

Για να επιτρέψετε σε εξωτερικούς χρήστες να στέλνουν μηνύματα ηλεκτρονικού ταχυδρομείου σε αυτόν τον δημόσιο φάκελο, προσθέστε την πρόσβαση CreateItems δικαίωμα στο χρήστη Ανώνυμος. Για παράδειγμα, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .
