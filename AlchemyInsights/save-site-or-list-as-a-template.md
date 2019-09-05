---
title: Αποθήκευση τοποθεσίας ή λίστας ως προτύπου
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 1fe0a2f5bf65ef4e8cabf3d05a701c8eff966435
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36752032"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="37f58-102">Αποθήκευση τοποθεσίας ή λίστας ως προτύπου</span><span class="sxs-lookup"><span data-stu-id="37f58-102">Save site or list as a template</span></span>

<span data-ttu-id="37f58-103">Τα πρότυπα τοποθεσίας του SharePoint είναι προκατασκευά ορισμοί σχεδιασμένα γύρω από μια συγκεκριμένη επιχειρηματική ανάγκη.</span><span class="sxs-lookup"><span data-stu-id="37f58-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="37f58-104">Για περισσότερες πληροφορίες, ανατρέξτε [στο στοιχείο χρήση προτύπων για να δημιουργήσετε διαφορετικά είδη τοποθεσιών του SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="37f58-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="37f58-105">Ακολουθούν ορισμένα συνηθισμένα ζητήματα/λύσεις σχετικά με την αποθήκευση μιας τοποθεσίας ή λίστας ως προτύπου στο SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="37f58-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="37f58-106">**Το κουμπί αποθήκευσης προτύπου τοποθεσίας/λίστας δεν είναι διαθέσιμο ή λείπει**.</span><span class="sxs-lookup"><span data-stu-id="37f58-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="37f58-107">Οι διαχειριστές θα πρέπει να επιτρέπουν προσαρμοσμένη δέσμη ενεργειών για να ενεργοποιήσετε τις δυνατότητες του προτύπου.</span><span class="sxs-lookup"><span data-stu-id="37f58-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="37f58-108">Για λεπτομερή βήματα, παραδείγματα και θέματα, δείτε να [επιτρέπεται ή να αποτρέπεται η προσαρμοσμένη δέσμη ενεργειών](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="37f58-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="37f58-109">Η εντολή "Αποθήκευση τοποθεσίας ως προτύπου" δεν υποστηρίζεται και μπορεί να προκαλέσει προβλήματα σε τοποθεσίες που χρησιμοποιούν την υποδομή δημοσίευσης του SharePoint Server.</span><span class="sxs-lookup"><span data-stu-id="37f58-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="37f58-110">**Δεν είναι δυνατή η δημιουργία του προτύπου τοποθεσίας ή δεν λειτουργεί σωστά**</span><span class="sxs-lookup"><span data-stu-id="37f58-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="37f58-111">Το πρότυπο ενδέχεται να λείπει μια [δυνατότητα](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) και να μην ενεργοποιείται.</span><span class="sxs-lookup"><span data-stu-id="37f58-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="37f58-112">Εάν η δυνατότητα δεν είναι διαθέσιμη για ενεργοποίηση στην τρέχουσα συλλογή τοποθεσιών, δεν μπορείτε να χρησιμοποιήσετε το πρότυπο τοποθεσίας για να δημιουργήσετε μια τοποθεσία.</span><span class="sxs-lookup"><span data-stu-id="37f58-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="37f58-113">Ελέγξτε αν υπάρχουν λίστες ή βιβλιοθήκες που υπερβαίνουν τη [λίστα όριο προβολή](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) ορίου 5000 στοιχείων, καθώς αυτό μπορεί να αποκλείσει τη δημιουργία ενός προτύπου τοποθεσίας.</span><span class="sxs-lookup"><span data-stu-id="37f58-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="37f58-114">Η τοποθεσία ενδέχεται να χρησιμοποιεί πάρα πολλούς πόρους και επομένως το πρότυπο τοποθεσίας υπερβαίνει το όριο των 50 megabyte (MB).</span><span class="sxs-lookup"><span data-stu-id="37f58-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="37f58-115">Υπάρχουν προβλήματα με την εμφάνιση δεδομένων από μια λίστα που χρησιμοποιεί μια στήλη αναζήτησης.</span><span class="sxs-lookup"><span data-stu-id="37f58-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="37f58-116">Για περισσότερες πληροφορίες, δείτε [τη λίστα που δημιουργείται από το πρότυπο δεν εμφανίζει δεδομένα από τη σωστή λίστα αναζήτησης στο SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="37f58-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>


<span data-ttu-id="37f58-117">Για λεπτομερέστερες πληροφορίες σχετικά με κοινά προβλήματα και λύσεις, παρακαλούμε να αναφέρετε, να [δημιουργήσετε και να χρησιμοποιήσετε πρότυπα τοποθεσίας](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="37f58-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

