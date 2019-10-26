---
title: Dynamics 365-λάθος πίνακας ελέγχου εμφανίζεται στο Dynamics 365 ενοποιημένη διασύνδεση
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 3d7258bdd7366f679b048e93926ab7dfe0b956d9
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 10/25/2019
ms.locfileid: "36528551"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="e2254-102">Εμφανίζεται λάθος πίνακα εργαλείων στο Dynamics 365 ενοποιημένη διασύνδεση</span><span class="sxs-lookup"><span data-stu-id="e2254-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="e2254-103">Υπάρχουν διάφοροι λόγοι για τους οποίους ενδέχεται να δείτε έναν διαφορετικό πίνακα εργαλείων από αυτόν που αναμένετε:</span><span class="sxs-lookup"><span data-stu-id="e2254-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="e2254-104">Ο χρήστης έχει ορίσει έναν προεπιλεγμένο πίνακα εργαλείων χρήστη</span><span class="sxs-lookup"><span data-stu-id="e2254-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="e2254-105">Συνήθως, μπορείτε να αναγνωρίσετε έναν προεπιλεγμένο πίνακα εργαλείων χρήστη, εάν το κουμπί " **Ορισμός ως προεπιλεγμένου** " δεν εμφανίζεται στη γραμμή εντολών του πίνακα εργαλείων.</span><span class="sxs-lookup"><span data-stu-id="e2254-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="e2254-106">Ο προεπιλεγμένος πίνακας εργαλείων χρήστη θα παρακάμψει όλους τους άλλους προεπιλεγμένους πίνακες εργαλείων, ακόμα και αν ο προεπιλεγμένος πίνακας εργαλείων του χρήστη δεν βρίσκεται στην τρέχουσα εφαρμογή.</span><span class="sxs-lookup"><span data-stu-id="e2254-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="e2254-107">Χρησιμοποιήστε την ακόλουθη λύση για να καταργήσετε τον προεπιλεγμένο πίνακα εργαλείων.</span><span class="sxs-lookup"><span data-stu-id="e2254-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="e2254-108">Δημιουργήστε έναν νέο προσωπικό πίνακα εργαλείων.</span><span class="sxs-lookup"><span data-stu-id="e2254-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="e2254-109">Ορίστε αυτόν τον νέο πίνακα εργαλείων ως προεπιλεγμένο χρήστη.</span><span class="sxs-lookup"><span data-stu-id="e2254-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="e2254-110">Διαγράψτε αυτόν τον πίνακα εργαλείων.</span><span class="sxs-lookup"><span data-stu-id="e2254-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="e2254-111">Ο πίνακας εργαλείων έχει οριστεί στον χάρτη τοποθεσίας</span><span class="sxs-lookup"><span data-stu-id="e2254-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="e2254-112">Μπορεί να έχετε ορίσει έναν προεπιλεγμένο πίνακα εργαλείων εταιρείας, επιλέγοντας έναν πίνακα εργαλείων και επιλέγοντας "Ορισμός ως προεπιλογής" στην ενότητα "προσαρμογή του συστήματος".</span><span class="sxs-lookup"><span data-stu-id="e2254-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="e2254-113">Ωστόσο, ο πίνακας εργαλείων που ορίζεται στη σχεδίαση χάρτη τοποθεσίας θα προηγείται αυτού του πίνακα εργαλείων, εάν ο χρήστης έχει πρόσβαση σε αυτό.</span><span class="sxs-lookup"><span data-stu-id="e2254-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="e2254-114">Για να βλέπουν οι χρήστες τον πίνακα εργαλείων που έχετε ορίσει ως προεπιλεγμένο του οργανισμού, μπορείτε είτε:</span><span class="sxs-lookup"><span data-stu-id="e2254-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="e2254-115">Ορισμός αυτού του πίνακα εργαλείων στον χάρτη τοποθεσίας</span><span class="sxs-lookup"><span data-stu-id="e2254-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="e2254-116">Κατάργηση πρόσβασης στον πίνακα εργαλείων που ορίστηκε για αυτούς τους χρήστες</span><span class="sxs-lookup"><span data-stu-id="e2254-116">Remove access to the sitemap defined dashboard for those users</span></span>
