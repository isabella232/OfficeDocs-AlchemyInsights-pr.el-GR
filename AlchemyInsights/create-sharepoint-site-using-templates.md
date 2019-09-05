---
title: Δημιουργία τοποθεσίας στο SharePoint Online
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 42430c8dadc17b87dc7741f3fa045ba7c25fab84
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36755308"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="89804-102">Δημιουργία τοποθεσιών του SharePoint με χρήση προτύπων</span><span class="sxs-lookup"><span data-stu-id="89804-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="89804-103">Τα πρότυπα τοποθεσίας του SharePoint είναι προκατασκευά ορισμοί σχεδιασμένα γύρω από μια συγκεκριμένη επιχειρηματική ανάγκη.</span><span class="sxs-lookup"><span data-stu-id="89804-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="89804-104">Για περισσότερες πληροφορίες, ανατρέξτε [στο στοιχείο χρήση προτύπων για να δημιουργήσετε διαφορετικά είδη τοποθεσιών του SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="89804-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="89804-105">Ακολουθούν ορισμένα συνηθισμένα ζητήματα/λύσεις σχετικά με την αποθήκευση μιας τοποθεσίας ή λίστας ως προτύπου στο SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="89804-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="89804-106">**Το κουμπί αποθήκευσης προτύπου τοποθεσίας/λίστας δεν είναι διαθέσιμο ή λείπει**</span><span class="sxs-lookup"><span data-stu-id="89804-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="89804-107">Οι διαχειριστές θα πρέπει να επιτρέπουν προσαρμοσμένη δέσμη ενεργειών για να ενεργοποιήσετε τις δυνατότητες του προτύπου.</span><span class="sxs-lookup"><span data-stu-id="89804-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="89804-108">Για λεπτομερή βήματα, παραδείγματα και θέματα, βλέπε</span><span class="sxs-lookup"><span data-stu-id="89804-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="89804-109">Αποδοχή ή αποτροπή προσαρμοσμένης δέσμης ενεργειών</span><span class="sxs-lookup"><span data-stu-id="89804-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="89804-110">Η εντολή "Αποθήκευση τοποθεσίας ως προτύπου" δεν υποστηρίζεται και μπορεί να προκαλέσει προβλήματα σε τοποθεσίες που χρησιμοποιούν την υποδομή δημοσίευσης του SharePoint Server.</span><span class="sxs-lookup"><span data-stu-id="89804-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="89804-111">**Δεν είναι δυνατή η δημιουργία του προτύπου τοποθεσίας ή δεν λειτουργεί σωστά**</span><span class="sxs-lookup"><span data-stu-id="89804-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="89804-112">Το πρότυπο ενδέχεται να λείπει μια [δυνατότητα](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) και να μην ενεργοποιείται.</span><span class="sxs-lookup"><span data-stu-id="89804-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="89804-113">Εάν η δυνατότητα δεν είναι διαθέσιμη για ενεργοποίηση στην τρέχουσα συλλογή τοποθεσιών, δεν μπορείτε να χρησιμοποιήσετε το πρότυπο τοποθεσίας για να δημιουργήσετε μια τοποθεσία.</span><span class="sxs-lookup"><span data-stu-id="89804-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="89804-114">Ελέγξτε αν υπάρχουν λίστες ή βιβλιοθήκες που υπερβαίνουν τη [λίστα όριο προβολή](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) ορίου 5000 στοιχείων, καθώς αυτό μπορεί να αποκλείσει τη δημιουργία ενός προτύπου τοποθεσίας.</span><span class="sxs-lookup"><span data-stu-id="89804-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="89804-115">Η τοποθεσία ενδέχεται να χρησιμοποιεί πάρα πολλούς πόρους και επομένως το πρότυπο τοποθεσίας υπερβαίνει το όριο των 50 MB.</span><span class="sxs-lookup"><span data-stu-id="89804-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="89804-116">Υπάρχουν προβλήματα με την εμφάνιση δεδομένων από μια λίστα που χρησιμοποιεί μια στήλη αναζήτησης.</span><span class="sxs-lookup"><span data-stu-id="89804-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="89804-117">Για περισσότερες πληροφορίες, δείτε [τη λίστα που δημιουργείται από το πρότυπο δεν εμφανίζει δεδομένα από τη σωστή λίστα αναζήτησης στο SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="89804-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="89804-118">Για λεπτομερέστερες πληροφορίες σχετικά με κοινά προβλήματα και λύσεις, ελέγξτε τη [δημιουργία και τη χρήση προτύπων τοποθεσίας](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="89804-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



