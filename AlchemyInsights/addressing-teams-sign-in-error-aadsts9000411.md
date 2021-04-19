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
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a><span data-ttu-id="5f451-102">Σφάλμα κατά την είσοδο στο Teams AADSTS9000411</span><span class="sxs-lookup"><span data-stu-id="5f451-102">Addressing Teams sign-in error AADSTS9000411</span></span>

<span data-ttu-id="5f451-103">Κατά την είσοδο στο Microsoft Teams, ενδέχεται να εμφανιστεί το σφάλμα: Λυπούμαστε, αλλά αντιμετωπίζετε πρόβλημα με την είσοδό σας **στο AADSTS9000411: Η αίτηση δεν έχει μορφοποιηθεί σωστά. Η παράμετρος "login_hint" είναι διπλότυπη.**</span><span class="sxs-lookup"><span data-stu-id="5f451-103">When signing in to Microsoft Teams, you may receive the error: **Sorry, but we're having trouble with signing you in AADSTS9000411: The request is not properly formatted. The parameter "login_hint" is duplicated.**</span></span>

<span data-ttu-id="5f451-104">Για να αντιμετωπίσει αυτό το πρόβλημα, βεβαιωθείτε ότι τα προγράμματα-πελάτες του Microsoft Teams είναι ενημερωμένα.</span><span class="sxs-lookup"><span data-stu-id="5f451-104">To address this issue, please ensure your Microsoft Teams clients are updated.</span></span> <span data-ttu-id="5f451-105">Για περισσότερες πληροφορίες σχετικά με την ενημέρωση του προγράμματος-πελάτη σας, ανατρέξτε [στο θέμα Ενημέρωση του Microsoft Teams.](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)</span><span class="sxs-lookup"><span data-stu-id="5f451-105">For more information on updating your client, see [Update Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

<span data-ttu-id="5f451-106">Εάν δεν μπορείτε να ενημερώσετε το πρόγραμμα-πελάτη για κάποιο λόγο, η αποσύνδεση από το πρόγραμμα-πελάτη θα εκκαθαρίσει τα περισσότερα δεδομένα στο cache.</span><span class="sxs-lookup"><span data-stu-id="5f451-106">If you cannot update your client for some reason, logging off the client will clear most cached data.</span></span> <span data-ttu-id="5f451-107">Ωστόσο, εάν εξακολουθείτε να έχετε προβλήματα μετά την αποσύνδεση/σύνδεση, κλείστε το Teams και κάντε εκκαθάριση του cache του προγράμματος-πελάτη, κάνοντας τα εξής:</span><span class="sxs-lookup"><span data-stu-id="5f451-107">However, if you still have issues after logoff/logon, quit Teams and please clear your client cache by doing the following:</span></span>
1. <span data-ttu-id="5f451-108">Κλείστε το Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="5f451-108">Close Microsoft Teams.</span></span>
2. <span data-ttu-id="5f451-109">Μεταβείτε στο: %appdata%\microsoft\teams και διαγράψτε όλα τα αρχεία.</span><span class="sxs-lookup"><span data-stu-id="5f451-109">Go to: %appdata%\microsoft\teams and delete all the files.</span></span>
3. <span data-ttu-id="5f451-110">Ανοίξτε ξανά το Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="5f451-110">Reopen Microsoft Teams.</span></span>
