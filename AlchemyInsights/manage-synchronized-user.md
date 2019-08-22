---
title: Διαχείριση χρήστη συγχρονίζονται
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: a943c59d67c512e6326856dacd0053db121f6aa3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36541990"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a>Δεν είναι δυνατό να ορίσετε την κύρια διεύθυνση ηλεκτρονικού ταχυδρομείου ή να αλλάξετε τα χαρακτηριστικά χρήστη

Εάν είναι ενεργοποιημένη η συγχρονισμού καταλόγου για το περιβάλλον σας, ορισμένα χαρακτηριστικά του χρήστη ή το αντικείμενο δεν μπορεί να αλλάξει χρησιμοποιώντας το Κέντρο διαχείρισης Microsoft 365.

Για να διαχειρίζονται πλήρως συγχρονισμένη χρήστες και όλα τα χαρακτηριστικά τους, χρησιμοποιήσετε την τοπική υπηρεσία καταλόγου active directory χρήστες και ομάδες Κονσόλα διαχείρισης (adsiedit.msc).  

Εναλλακτικά, μπορείτε να αλλάξετε μεμονωμένους χρήστες ή χαρακτηριστικών για συγχρονισμένες χρήστες χρησιμοποιώντας powershell, όπως φαίνεται σε αυτά τα κοινά παραδείγματα: 
- Σύνολο MsolUser - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com
- Σύνολο-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com" - DisplayName "Δοκιμής χρήστη" - Επώνυμο "Χρήστης"-τον τίτλο "Διευθυντής"-τμήμα "HR"
- Κατάργηση-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com