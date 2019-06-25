---
title: Δημιουργία τοποθεσίας στο SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 9ab06cbd1648da31d8a04e61c237a2326b4bbe93
ms.sourcegitcommit: f856d46a325c517fc29d935c27f21b77c4219e66
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/24/2019
ms.locfileid: "35199273"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="7f54e-102">Δημιουργία τοποθεσιών του SharePoint, χρησιμοποιώντας τα πρότυπα</span><span class="sxs-lookup"><span data-stu-id="7f54e-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="7f54e-103">Τα πρότυπα τοποθεσίας του SharePoint είναι προκατασκευασμένες ορισμοί σχεδιασμένο γύρω από μια συγκεκριμένη επιχειρηματική ανάγκη.</span><span class="sxs-lookup"><span data-stu-id="7f54e-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="7f54e-104">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Χρήση πρότυπα για να δημιουργήσετε διαφορετικά είδη των τοποθεσιών του SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="7f54e-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="7f54e-105">Ακολουθούν ορισμένα κοινά θέματα/λύσεις σχετικά με την αποθήκευση μιας τοποθεσίας ή λίστας ως πρότυπο στο Sharepoint Online.</span><span class="sxs-lookup"><span data-stu-id="7f54e-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="7f54e-106">**"Πρότυπο" τοποθεσία/λίστα Αποθήκευση "δεν είναι διαθέσιμη ή δεν υπάρχει**</span><span class="sxs-lookup"><span data-stu-id="7f54e-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="7f54e-107">Οι διαχειριστές θα πρέπει να επιτρέψει προσαρμοσμένης δέσμης ενεργειών για να ενεργοποιήσετε τις δυνατότητες του προτύπου.</span><span class="sxs-lookup"><span data-stu-id="7f54e-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="7f54e-108">Για λεπτομερή βήματα, δείτε παραδείγματα και θέματα</span><span class="sxs-lookup"><span data-stu-id="7f54e-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="7f54e-109">Ύπαρξη ή απαγόρευση της προσαρμοσμένης δέσμης ενεργειών</span><span class="sxs-lookup"><span data-stu-id="7f54e-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="7f54e-110">Την αποθήκευση τοποθεσίας ως πρότυπο εντολή δεν υποστηρίζεται και μπορεί να προκαλέσει προβλήματα σε τοποθεσίες που χρησιμοποιούν την υποδομή δημοσίευσης του SharePoint Server.</span><span class="sxs-lookup"><span data-stu-id="7f54e-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="7f54e-111">**Το πρότυπο τοποθεσίας δεν είναι δυνατό να δημιουργηθεί ή δεν λειτουργεί σωστά**</span><span class="sxs-lookup"><span data-stu-id="7f54e-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="7f54e-112">Το πρότυπο ενδέχεται να μην διαθέτει μια [δυνατότητα](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) και δεν θα ενεργοποιήσετε.</span><span class="sxs-lookup"><span data-stu-id="7f54e-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="7f54e-113">Εάν η δυνατότητα δεν είναι διαθέσιμη για την ενεργοποίηση της τρέχουσας συλλογής τοποθεσιών, μπορείτε να χρησιμοποιήσετε το πρότυπο τοποθεσίας για να δημιουργήσετε μια τοποθεσία.</span><span class="sxs-lookup"><span data-stu-id="7f54e-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="7f54e-114">Ελέγξτε για να δείτε εάν οποιεσδήποτε λίστες ή βιβλιοθήκες υπερβαίνει το [Όριο προβολής λίστας που όριο](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 στοιχεία όπως αυτό μπορεί να αποκλείσει τη δημιουργία ενός προτύπου τοποθεσίας.</span><span class="sxs-lookup"><span data-stu-id="7f54e-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="7f54e-115">Η τοποθεσία μπορεί να χρησιμοποιεί πάρα πολλούς πόρους και επομένως το πρότυπο τοποθεσίας υπερβαίνει το όριο των 50 MB.</span><span class="sxs-lookup"><span data-stu-id="7f54e-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="7f54e-116">Υπάρχουν προβλήματα που εμφανίζουν δεδομένα από μια λίστα που χρησιμοποιεί μια στήλη αναζήτησης.</span><span class="sxs-lookup"><span data-stu-id="7f54e-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="7f54e-117">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [που δημιουργείται από το πρότυπο λίστας δεν εμφανίζει τα δεδομένα από τη λίστα αναζήτησης σωστά στο SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span><span class="sxs-lookup"><span data-stu-id="7f54e-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span></span>

<span data-ttu-id="7f54e-118">Για πιο λεπτομερείς πληροφορίες σχετικά με προβλήματα και λύσεις, δείτε [Δημιουργία και χρήση προτύπων τοποθεσίας](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="7f54e-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



