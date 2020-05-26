---
title: Αντιμετώπιση ομάδων εισόδου σφάλμα AADSTS9000411
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: b70f1320ea1dfa29e6fa489bd02acfcd1d92971b
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 05/20/2020
ms.locfileid: "44357549"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>Αντιμετώπιση ομάδων εισόδου σφάλμα AADSTS9000411

Κατά την είσοδο στο Microsoft Teams, ενδέχεται να λάβετε το σφάλμα: **Λυπούμαστε, αλλά αντιμετωπίζουμε προβλήματα με την υπογραφή σας στο AADSTS9000411: Η αίτηση δεν έχει μορφοποιηθεί σωστά. Η παράμετρος "login_hint" αναπαράγεται.**

Για να αντιμετωπίσετε αυτό το ζήτημα, βεβαιωθείτε ότι τα προγράμματα-πελάτες του Microsoft Teams ενημερώνονται. Για περισσότερες πληροφορίες σχετικά με την ενημέρωση του υπολογιστή-πελάτη, ανατρέξτε στο θέμα [Ενημέρωση ομάδων της Microsoft](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

Εάν δεν μπορείτε να ενημερώσετε τον υπολογιστή-πελάτη για κάποιο λόγο, η αποσύνδεση του υπολογιστή-πελάτη θα καταργήσει τα περισσότερα προσωρινά αποθηκευμένα δεδομένα. Ωστόσο, εάν εξακολουθείτε να έχετε προβλήματα μετά την αποσύνδεση/σύνδεση, κλείστε το αρχείο teams και καταργήστε την προσωρινή μνήμη του υπολογιστή-πελάτη, κάνοντας τα εξής:
1. Κλείστε τις ομάδες της Microsoft.
2. Μεταβείτε στη διεύθυνση: %appdata%\microsoft\teams και διαγράψτε όλα τα αρχεία.
3. Ανοίξτε ξανά τις ομάδες της Microsoft.
