---
title: Αντιμετώπιση Teams σφάλματος είσοδος AADSTS9000411
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
ms.openlocfilehash: 883bf48d3628702c92361a5250f0d59e1352918349b8bc6c3eae5a948b72fc57
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53953024"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>Αντιμετώπιση Teams σφάλματος είσοδος AADSTS9000411

Κατά την είσοδο στο Microsoft Teams, ενδέχεται να εμφανιστεί το σφάλμα: Λυπούμαστε, αλλά αντιμετωπίζετε πρόβλημα με την είσοδό σας **στο AADSTS9000411: Η αίτηση δεν έχει μορφοποιηθεί σωστά. Η παράμετρος "login_hint" είναι διπλότυπη.**

Για να αντιμετωπίσει αυτό το πρόβλημα, βεβαιωθείτε ότι τα Microsoft Teams σας ενημερώνονται. Για περισσότερες πληροφορίες σχετικά με την ενημέρωση του προγράμματος-πελάτη σας, [ανατρέξτε στο θέμα Microsoft Teams.](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)

Εάν δεν μπορείτε να ενημερώσετε το πρόγραμμα-πελάτη για κάποιο λόγο, η αποσύνδεση από το πρόγραμμα-πελάτη θα εκκαθαρίσει τα περισσότερα δεδομένα στο cache. Ωστόσο, εάν εξακολουθείτε να έχετε προβλήματα μετά την αποσύνδεση/σύνδεση, κλείστε το Teams και κάντε εκκαθάριση του cache του προγράμματος-πελάτη, κάνοντας τα εξής:
1. Κλείστε Microsoft Teams.
2. Μεταβείτε στο: %appdata%\microsoft\teams και διαγράψτε όλα τα αρχεία.
3. Ανοίξτε ξανά Microsoft Teams.
