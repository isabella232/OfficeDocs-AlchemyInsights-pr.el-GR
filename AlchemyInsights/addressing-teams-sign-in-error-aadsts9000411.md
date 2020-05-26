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
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a><span data-ttu-id="7b8bd-102">Αντιμετώπιση ομάδων εισόδου σφάλμα AADSTS9000411</span><span class="sxs-lookup"><span data-stu-id="7b8bd-102">Addressing Teams sign-in error AADSTS9000411</span></span>

<span data-ttu-id="7b8bd-103">Κατά την είσοδο στο Microsoft Teams, ενδέχεται να λάβετε το σφάλμα: **Λυπούμαστε, αλλά αντιμετωπίζουμε προβλήματα με την υπογραφή σας στο AADSTS9000411: Η αίτηση δεν έχει μορφοποιηθεί σωστά. Η παράμετρος "login_hint" αναπαράγεται.**</span><span class="sxs-lookup"><span data-stu-id="7b8bd-103">When signing in to Microsoft Teams, you may receive the error: **Sorry, but we're having trouble with signing you in AADSTS9000411: The request is not properly formatted. The parameter "login_hint" is duplicated.**</span></span>

<span data-ttu-id="7b8bd-104">Για να αντιμετωπίσετε αυτό το ζήτημα, βεβαιωθείτε ότι τα προγράμματα-πελάτες του Microsoft Teams ενημερώνονται.</span><span class="sxs-lookup"><span data-stu-id="7b8bd-104">To address this issue, please ensure your Microsoft Teams clients are updated.</span></span> <span data-ttu-id="7b8bd-105">Για περισσότερες πληροφορίες σχετικά με την ενημέρωση του υπολογιστή-πελάτη, ανατρέξτε στο θέμα [Ενημέρωση ομάδων της Microsoft](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="7b8bd-105">For more information on updating your client, see [Update Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

<span data-ttu-id="7b8bd-106">Εάν δεν μπορείτε να ενημερώσετε τον υπολογιστή-πελάτη για κάποιο λόγο, η αποσύνδεση του υπολογιστή-πελάτη θα καταργήσει τα περισσότερα προσωρινά αποθηκευμένα δεδομένα.</span><span class="sxs-lookup"><span data-stu-id="7b8bd-106">If you cannot update your client for some reason, logging off the client will clear most cached data.</span></span> <span data-ttu-id="7b8bd-107">Ωστόσο, εάν εξακολουθείτε να έχετε προβλήματα μετά την αποσύνδεση/σύνδεση, κλείστε το αρχείο teams και καταργήστε την προσωρινή μνήμη του υπολογιστή-πελάτη, κάνοντας τα εξής:</span><span class="sxs-lookup"><span data-stu-id="7b8bd-107">However, if you still have issues after logoff/logon, quit Teams and please clear your client cache by doing the following:</span></span>
1. <span data-ttu-id="7b8bd-108">Κλείστε τις ομάδες της Microsoft.</span><span class="sxs-lookup"><span data-stu-id="7b8bd-108">Close Microsoft Teams.</span></span>
2. <span data-ttu-id="7b8bd-109">Μεταβείτε στη διεύθυνση: %appdata%\microsoft\teams και διαγράψτε όλα τα αρχεία.</span><span class="sxs-lookup"><span data-stu-id="7b8bd-109">Go to: %appdata%\microsoft\teams and delete all the files.</span></span>
3. <span data-ttu-id="7b8bd-110">Ανοίξτε ξανά τις ομάδες της Microsoft.</span><span class="sxs-lookup"><span data-stu-id="7b8bd-110">Reopen Microsoft Teams.</span></span>
