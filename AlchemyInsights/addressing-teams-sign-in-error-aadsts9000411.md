---
title: Σφάλμα κατά την είσοδο στο Teams AADSTS9000411
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: 7b0e90e3fea716df649ec906ad8b3008386684be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821987"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>Σφάλμα κατά την είσοδο στο Teams AADSTS9000411

Κατά την είσοδο στο Microsoft Teams, ενδέχεται να εμφανιστεί το σφάλμα: Λυπούμαστε, αλλά αντιμετωπίζετε πρόβλημα με την είσοδό σας **στο AADSTS9000411: Η αίτηση δεν έχει μορφοποιηθεί σωστά. Η παράμετρος "login_hint" είναι διπλότυπη.**

Για να αντιμετωπίσει αυτό το πρόβλημα, βεβαιωθείτε ότι τα προγράμματα-πελάτες του Microsoft Teams είναι ενημερωμένα. Για περισσότερες πληροφορίες σχετικά με την ενημέρωση του προγράμματος-πελάτη σας, ανατρέξτε [στο θέμα Ενημέρωση του Microsoft Teams.](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)

Εάν δεν μπορείτε να ενημερώσετε το πρόγραμμα-πελάτη για κάποιο λόγο, η αποσύνδεση από το πρόγραμμα-πελάτη θα εκκαθαρίσει τα περισσότερα δεδομένα στο cache. Ωστόσο, εάν εξακολουθείτε να έχετε προβλήματα μετά την αποσύνδεση/σύνδεση, κλείστε το Teams και κάντε εκκαθάριση του cache του προγράμματος-πελάτη, κάνοντας τα εξής:
1. Κλείστε το Microsoft Teams.
2. Μεταβείτε στο: %appdata%\microsoft\teams και διαγράψτε όλα τα αρχεία.
3. Ανοίξτε ξανά το Microsoft Teams.
