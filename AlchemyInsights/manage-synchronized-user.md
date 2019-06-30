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
ms.openlocfilehash: 5a383bdd17c5fa055c35a923ca36e0e0f6d429e4
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35380505"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a>Δεν είναι δυνατό να ορίσετε την κύρια διεύθυνση ηλεκτρονικού ταχυδρομείου ή να αλλάξετε τα χαρακτηριστικά χρήστη

Εάν είναι ενεργοποιημένη η συγχρονισμού καταλόγου για το περιβάλλον σας ορισμένα χαρακτηριστικά χρήστης ή το αντικείμενο δεν μπορεί να αλλάξει χρησιμοποιώντας το Κέντρο διαχείρισης.
Για να διαχειρίζονται πλήρως συγχρονισμένη χρήστες και όλα τα χαρακτηριστικά τους, χρησιμοποιήσετε την τοπική υπηρεσία καταλόγου active directory χρήστες και ομάδες Κονσόλα διαχείρισης (adsiedit.msc).  

Εναλλακτικά, μπορείτε να αλλάξετε μεμονωμένους χρήστες ή χαρακτηριστικών για συγχρονισμένες χρήστες χρησιμοποιώντας powershell, όπως φαίνεται σε αυτά τα κοινά παραδείγματα: 
- Σύνολο MsolUser - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com
- Σύνολο-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com" - DisplayName "Δοκιμής χρήστη" - Επώνυμο "Χρήστης"-τον τίτλο "Διευθυντής"-τμήμα "HR"
- Κατάργηση-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com