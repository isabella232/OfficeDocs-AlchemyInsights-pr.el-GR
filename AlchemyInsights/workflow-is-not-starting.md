---
title: Δεν γίνεται εκκίνηση της ροής εργασίας
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 8/2/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: d4bfdb44c04eb6838f4a265e55a4873d14c78f6d
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36557972"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="b5da0-102">Δεν γίνεται εκκίνηση της ροής εργασίας</span><span class="sxs-lookup"><span data-stu-id="b5da0-102">Workflow is not starting</span></span>

- <span data-ttu-id="b5da0-103">Ροές εργασίας SharePoint 2010 και το 2013 του SharePoint δεν το αρχικό.</span><span class="sxs-lookup"><span data-stu-id="b5da0-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="b5da0-104">Εάν δεν ξεκινά η ροή εργασιών σας, ίσως υπάρχει κάποιο ζήτημα προσωρινής υπηρεσίας όπου οι χρήστες ενδέχεται να αντιμετωπίζουν περιστασιακές καθυστερήσεις με την εξέλιξη της ροής εργασίας.</span><span class="sxs-lookup"><span data-stu-id="b5da0-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="b5da0-105">Ελέγξτε το [Πίνακας εργαλείων υγείας εξυπηρέτησης](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) για να δείτε εάν ο οργανισμός σας επηρεάζεται.</span><span class="sxs-lookup"><span data-stu-id="b5da0-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="b5da0-106">Εάν έχουν περάσει περισσότερες από 24 ώρες, από τη στιγμή που είδατε πρώτα αυτό το ζήτημα, συνδεθείτε ένα εισιτήριο υποστήριξης.</span><span class="sxs-lookup"><span data-stu-id="b5da0-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="b5da0-107">Σε πολλές περιπτώσεις, εργαζόμαστε ήδη σε μια λύση.</span><span class="sxs-lookup"><span data-stu-id="b5da0-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="b5da0-108">Παρακαλούμε να μας δώσετε τουλάχιστον 24 ώρες για να ολοκληρωθεί μια λύση.</span><span class="sxs-lookup"><span data-stu-id="b5da0-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="b5da0-109">Ροές εργασίας SharePoint 2010 καθυστέρηση στην εκκίνηση.</span><span class="sxs-lookup"><span data-stu-id="b5da0-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="b5da0-110">Αυτό συμβαίνει εάν η ροή εργασίας ενεργοποιείται σε μεγάλες δέσμες.</span><span class="sxs-lookup"><span data-stu-id="b5da0-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="b5da0-111">(για παράδειγμα, όταν πολλά στοιχεία προστίθενται ταυτόχρονα).</span><span class="sxs-lookup"><span data-stu-id="b5da0-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="b5da0-112">Ροές εργασίας δεν έχει σχεδιαστεί για να εκτελούνται σε πραγματικό χρόνο, επομένως μια καθυστέρηση είναι η συμπεριφορά οφείλεται στη σχεδίαση.</span><span class="sxs-lookup"><span data-stu-id="b5da0-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="b5da0-113">Εάν η ροή εργασίας είναι πολύπλοκη γλώσσας Extensible Markup αντικειμένου (XMOL), η μεταγλώττιση μπορεί να είναι αργή.</span><span class="sxs-lookup"><span data-stu-id="b5da0-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="b5da0-114">Ελέγξτε [αυτό](https://support.microsoft.com/en-us/kb/3043697) το άρθρο.</span><span class="sxs-lookup"><span data-stu-id="b5da0-114">Check [this](https://support.microsoft.com/en-us/kb/3043697) article.</span></span>

    - <span data-ttu-id="b5da0-115">Θα πρέπει να απλοποιήσετε τη ροή εργασίας ή να ξανασχεδιάσετε χρησιμοποιώντας τον τύπο πλατφόρμας ροής εργασίας του Microsoft SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="b5da0-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="b5da0-116">Το ιστορικό της ροής εργασίας σας έχει γίνει μεγάλη, μπορεί να θέλετε να εκκαθάριση των στοιχείων ή να δημιουργήσετε μια νέα λίστα ιστορικού.</span><span class="sxs-lookup"><span data-stu-id="b5da0-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="b5da0-117">Περισσότερες πληροφορίες: [Εκκαθάριση ιστορικού ροής εργασίας](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="b5da0-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="b5da0-118">Σχετικά θέματα</span><span class="sxs-lookup"><span data-stu-id="b5da0-118">Related topics</span></span>
<span data-ttu-id="b5da0-119">Θέλετε να δοκιμάσετε τη ροή της Microsoft με την ηλεκτρονική του SharePoint;</span><span class="sxs-lookup"><span data-stu-id="b5da0-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="b5da0-120">Δημιουργία ροής</span><span class="sxs-lookup"><span data-stu-id="b5da0-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="b5da0-121">Του SharePoint και ροής</span><span class="sxs-lookup"><span data-stu-id="b5da0-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


