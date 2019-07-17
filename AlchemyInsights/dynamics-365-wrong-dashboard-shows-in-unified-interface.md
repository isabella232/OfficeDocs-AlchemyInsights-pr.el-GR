---
title: Dynamics 365 - λάθος πίνακα εργαλείων εμφανίζεται σε ενοποιημένη διασύνδεση Dynamics 365
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 6edf6fbae0174f3fa4d635c7a99e7daae1243b60
ms.sourcegitcommit: a413a0e27ef4ab8c484fa9fccff8bbef381c8b96
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35747709"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="ba4ac-102">Εμφανίζει λάθος πίνακα εργαλείων σε ενοποιημένη διασύνδεση Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="ba4ac-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="ba4ac-103">Υπάρχουν πολλές αιτίες γιατί μπορεί να δείτε ένα διαφορετικό πίνακα εργαλείων από αυτήν που αναμένετε:</span><span class="sxs-lookup"><span data-stu-id="ba4ac-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="ba4ac-104">Ο χρήστης έχει ορίσει προεπιλεγμένο πίνακα εργαλείων χρήστη</span><span class="sxs-lookup"><span data-stu-id="ba4ac-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="ba4ac-105">Συνήθως μπορείτε να αναγνωρίσετε ένα χρήστη έχει οριστεί προεπιλεγμένο πίνακα εργαλείων, εάν το κουμπί " **Ορισμός ως προεπιλογή** " δεν εμφανίζεται στη γραμμή εντολών του πίνακα εργαλείων.</span><span class="sxs-lookup"><span data-stu-id="ba4ac-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="ba4ac-106">Τον πίνακα εργαλείων του προεπιλεγμένου χρήστη θα αντικαταστήσει όλες άλλες προεπιλεγμένες πίνακες εργαλείων, ακόμη και αν ο χρήστης προεπιλεγμένου πίνακα εργαλείων δεν είναι η τρέχουσα εφαρμογή.</span><span class="sxs-lookup"><span data-stu-id="ba4ac-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="ba4ac-107">Χρησιμοποιήστε τις ακόλουθες εναλλακτικές λύσεις για την ακύρωση τους προεπιλεγμένο πίνακα εργαλείων.</span><span class="sxs-lookup"><span data-stu-id="ba4ac-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="ba4ac-108">Δημιουργία νέου προσωπικού πίνακα εργαλείων.</span><span class="sxs-lookup"><span data-stu-id="ba4ac-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="ba4ac-109">Ορίστε το νέο πίνακα εργαλείων ως τον προεπιλεγμένο χρήστη.</span><span class="sxs-lookup"><span data-stu-id="ba4ac-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="ba4ac-110">Η διαγραφή αυτού του πίνακα εργαλείων.</span><span class="sxs-lookup"><span data-stu-id="ba4ac-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="ba4ac-111">Ο πίνακας εργαλείων που έχει οριστεί στο sitemap</span><span class="sxs-lookup"><span data-stu-id="ba4ac-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="ba4ac-112">Ενδέχεται να έχετε ορίσει έναν πίνακα εργαλείων προεπιλεγμένη εταιρεία, επιλέγοντας έναν πίνακα εργαλείων και επιλέξτε "Ορισμός ως προεπιλογής" στην ενότητα 'Προσαρμογή του συστήματος'.</span><span class="sxs-lookup"><span data-stu-id="ba4ac-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="ba4ac-113">Αλλά ο πίνακας εργαλείων που ορίζονται στη σχεδίαση χάρτη τοποθεσίας θα έχουν προτεραιότητα έναντι αυτού του πίνακα εργαλείων, εάν ο χρήστης έχει πρόσβαση σε αυτό.</span><span class="sxs-lookup"><span data-stu-id="ba4ac-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="ba4ac-114">Για να έχουν οι χρήστες, δείτε τον πίνακα εργαλείων που έχετε ορίσει ως προεπιλεγμένο οργανισμό, μπορείτε είτε:</span><span class="sxs-lookup"><span data-stu-id="ba4ac-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="ba4ac-115">Ορισμός αυτού του πίνακα εργαλείων στο sitemap</span><span class="sxs-lookup"><span data-stu-id="ba4ac-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="ba4ac-116">Κατάργηση πρόσβασης στον πίνακα εργαλείων του χάρτη τοποθεσίας που έχουν οριστεί για αυτούς τους χρήστες</span><span class="sxs-lookup"><span data-stu-id="ba4ac-116">Remove access to the sitemap defined dashboard for those users</span></span>
