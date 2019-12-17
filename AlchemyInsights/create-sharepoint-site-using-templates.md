---
title: Δημιουργία τοποθεσίας στο SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 458990889d3c074820527982cbfa6e2d198d3e66
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052469"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="8c3c4-102">Δημιουργία τοποθεσιών του SharePoint με χρήση προτύπων</span><span class="sxs-lookup"><span data-stu-id="8c3c4-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="8c3c4-103">Τα πρότυπα τοποθεσίας του SharePoint είναι προκατασκευά ορισμοί σχεδιασμένα γύρω από μια συγκεκριμένη επιχειρηματική ανάγκη.</span><span class="sxs-lookup"><span data-stu-id="8c3c4-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="8c3c4-104">Για περισσότερες πληροφορίες, ανατρέξτε [στο στοιχείο χρήση προτύπων για να δημιουργήσετε διαφορετικά είδη τοποθεσιών του SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="8c3c4-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="8c3c4-105">Ακολουθούν ορισμένα συνηθισμένα ζητήματα/λύσεις σχετικά με την αποθήκευση μιας τοποθεσίας ή λίστας ως προτύπου στο SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="8c3c4-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="8c3c4-106">**Το κουμπί αποθήκευσης προτύπου τοποθεσίας/λίστας δεν είναι διαθέσιμο ή λείπει**</span><span class="sxs-lookup"><span data-stu-id="8c3c4-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="8c3c4-107">Οι διαχειριστές θα πρέπει να επιτρέπουν προσαρμοσμένη δέσμη ενεργειών για να ενεργοποιήσετε τις δυνατότητες του προτύπου.</span><span class="sxs-lookup"><span data-stu-id="8c3c4-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="8c3c4-108">Για λεπτομερή βήματα, παραδείγματα και θέματα, βλέπε</span><span class="sxs-lookup"><span data-stu-id="8c3c4-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="8c3c4-109">Αποδοχή ή αποτροπή προσαρμοσμένης δέσμης ενεργειών</span><span class="sxs-lookup"><span data-stu-id="8c3c4-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="8c3c4-110">Η εντολή "Αποθήκευση τοποθεσίας ως προτύπου" δεν υποστηρίζεται και μπορεί να προκαλέσει προβλήματα σε τοποθεσίες που χρησιμοποιούν την υποδομή δημοσίευσης του SharePoint Server.</span><span class="sxs-lookup"><span data-stu-id="8c3c4-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="8c3c4-111">**Δεν είναι δυνατή η δημιουργία του προτύπου τοποθεσίας ή δεν λειτουργεί σωστά**</span><span class="sxs-lookup"><span data-stu-id="8c3c4-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="8c3c4-112">Το πρότυπο ενδέχεται να λείπει μια [δυνατότητα](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) και να μην ενεργοποιείται.</span><span class="sxs-lookup"><span data-stu-id="8c3c4-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="8c3c4-113">Εάν η δυνατότητα δεν είναι διαθέσιμη για ενεργοποίηση στην τρέχουσα συλλογή τοποθεσιών, δεν μπορείτε να χρησιμοποιήσετε το πρότυπο τοποθεσίας για να δημιουργήσετε μια τοποθεσία.</span><span class="sxs-lookup"><span data-stu-id="8c3c4-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="8c3c4-114">Ελέγξτε αν υπάρχουν λίστες ή βιβλιοθήκες που υπερβαίνουν τη [λίστα όριο προβολή](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) ορίου 5000 στοιχείων, καθώς αυτό μπορεί να αποκλείσει τη δημιουργία ενός προτύπου τοποθεσίας.</span><span class="sxs-lookup"><span data-stu-id="8c3c4-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="8c3c4-115">Η τοποθεσία ενδέχεται να χρησιμοποιεί πάρα πολλούς πόρους και επομένως το πρότυπο τοποθεσίας υπερβαίνει το όριο των 50 MB.</span><span class="sxs-lookup"><span data-stu-id="8c3c4-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="8c3c4-116">Υπάρχουν προβλήματα με την εμφάνιση δεδομένων από μια λίστα που χρησιμοποιεί μια στήλη αναζήτησης.</span><span class="sxs-lookup"><span data-stu-id="8c3c4-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="8c3c4-117">Για περισσότερες πληροφορίες, δείτε [τη λίστα που δημιουργείται από το πρότυπο δεν εμφανίζει δεδομένα από τη σωστή λίστα αναζήτησης στο SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="8c3c4-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="8c3c4-118">Για λεπτομερέστερες πληροφορίες σχετικά με κοινά προβλήματα και λύσεις, ελέγξτε τη [δημιουργία και τη χρήση προτύπων τοποθεσίας](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="8c3c4-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



