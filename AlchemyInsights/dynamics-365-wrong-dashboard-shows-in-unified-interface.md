---
title: Dynamics 365-λανθασμένος πίνακας εργαλείων εμφανίζεται στο ενοποιημένο περιβάλλον εργασίας του Dynamics 365
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 02e33c7dbdfe9b7d2ad7a04f154cf067fba0aab2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711275"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="d06ea-102">Εμφανίζεται εσφαλμένος πίνακας εργαλείων στο ενοποιημένο περιβάλλον εργασίας του Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="d06ea-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="d06ea-103">Υπάρχουν διάφοροι λόγοι για τους οποίους μπορεί να δείτε έναν διαφορετικό πίνακα εργαλείων από αυτόν που αναμένετε:</span><span class="sxs-lookup"><span data-stu-id="d06ea-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="d06ea-104">Ο χρήστης έχει ρυθμίσει έναν προεπιλεγμένο πίνακα εργαλείων χρήστη</span><span class="sxs-lookup"><span data-stu-id="d06ea-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="d06ea-105">Συνήθως, μπορείτε να προσδιορίσετε ότι ο προεπιλεγμένος πίνακας εργαλείων του χρήστη έχει καθοριστεί, εάν το κουμπί " **ρύθμιση ως προεπιλογής** " δεν εμφανίζεται στη γραμμή εντολών του πίνακα εργαλείων.</span><span class="sxs-lookup"><span data-stu-id="d06ea-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="d06ea-106">Ο προεπιλεγμένος πίνακας εργαλείων χρήστη θα αντικαταστήσει όλους τους άλλους προεπιλεγμένους πίνακες εργαλείων, ακόμα και αν ο προεπιλεγμένος πίνακας εργαλείων του χρήστη δεν βρίσκεται στην τρέχουσα εφαρμογή.</span><span class="sxs-lookup"><span data-stu-id="d06ea-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="d06ea-107">Χρησιμοποιήστε την παρακάτω λύση για να κάνετε ακύρωση του προεπιλεγμένου πίνακα εργαλείων.</span><span class="sxs-lookup"><span data-stu-id="d06ea-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="d06ea-108">Δημιουργία νέου προσωπικού πίνακα εργαλείων.</span><span class="sxs-lookup"><span data-stu-id="d06ea-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="d06ea-109">Ορίστε αυτόν τον νέο πίνακα εργαλείων ως προεπιλεγμένο χρήστη.</span><span class="sxs-lookup"><span data-stu-id="d06ea-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="d06ea-110">Διαγράψτε αυτόν τον πίνακα εργαλείων.</span><span class="sxs-lookup"><span data-stu-id="d06ea-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="d06ea-111">Ο πίνακας εργαλείων έχει καθοριστεί στο χάρτη τοποθεσίας</span><span class="sxs-lookup"><span data-stu-id="d06ea-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="d06ea-112">Μπορεί να έχετε ρυθμίσει έναν προεπιλεγμένο πίνακα εργαλείων οργανισμού, επιλέγοντας έναν πίνακα εργαλείων και επιλέγοντας "Ορισμός ως προεπιλογής" στην περιοχή "προσαρμογή του συστήματος".</span><span class="sxs-lookup"><span data-stu-id="d06ea-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="d06ea-113">Αλλά ο πίνακας εργαλείων που καθορίζεται στο πρόγραμμα σχεδίασης Sitemap θα υπερισχύει αυτού του πίνακα εργαλείων, εάν ο χρήστης έχει πρόσβαση σε αυτό.</span><span class="sxs-lookup"><span data-stu-id="d06ea-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="d06ea-114">Για να βλέπουν οι χρήστες τον πίνακα εργαλείων που έχετε ρυθμίσει ως προεπιλογή του οργανισμού, μπορείτε να κάνετε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="d06ea-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="d06ea-115">Ορίστε αυτόν τον πίνακα εργαλείων στο χάρτη ιστοτόπου</span><span class="sxs-lookup"><span data-stu-id="d06ea-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="d06ea-116">Κατάργηση της πρόσβασης στον καθορισμένο πίνακα εργαλείων του χάρτη τοποθεσίας για αυτούς τους χρήστες</span><span class="sxs-lookup"><span data-stu-id="d06ea-116">Remove access to the sitemap defined dashboard for those users</span></span>
