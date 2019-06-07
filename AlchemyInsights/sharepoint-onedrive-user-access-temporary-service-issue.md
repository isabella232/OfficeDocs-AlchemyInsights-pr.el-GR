---
title: Ζητήματα επιδόσεων-SharePoint ή OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 745a62c917c0b94501843332d70609261c6d3b76
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34759151"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="d1295-102">Του SharePoint ή OneDrive αργή, μη προσβάσιμο ή μη διαθέσιμη για πολλούς χρήστες</span><span class="sxs-lookup"><span data-stu-id="d1295-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="d1295-103">Εάν μια τοποθεσία OneDrive ή SharePoint δεν είναι διαθέσιμες σε πολλούς χρήστες που προηγουμένως είχαν πρόσβαση, ίσως υπάρχει κάποιο ζήτημα προσωρινής υπηρεσίας.</span><span class="sxs-lookup"><span data-stu-id="d1295-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="d1295-104">[Ελέγξτε τον πίνακα εργαλείων υγείας υπηρεσία](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="d1295-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="d1295-105">Προσθέστε και άδεια χρήσης χρήστη</span><span class="sxs-lookup"><span data-stu-id="d1295-105">Add and license the user</span></span>

<span data-ttu-id="d1295-106">Βεβαιωθείτε ότι θα [αναθέσετε άδειες χρήσης σε χρήστες στο Office 365 για επιχειρήσεις](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="d1295-106">Ensure that you [Assign licenses to users in Office 365 for business](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span>


<span data-ttu-id="d1295-107">**Εκχώρηση δικαιωμάτων**</span><span class="sxs-lookup"><span data-stu-id="d1295-107">**Assign Permissions**</span></span>

<span data-ttu-id="d1295-108">Εάν ο χρήστης έχει αντιστοιχιστεί μια άδεια χρήσης του Sharepoint και εξακολουθεί να λαμβάνει ένα μήνυμα απαγόρευσης πρόσβασης, βεβαιωθείτε ότι να έχουν το [κατάλληλο επίπεδο δικαιωμάτων](https://docs.microsoft.com/sharepoint/understanding-permission-levels) που έχουν εκχωρηθεί.</span><span class="sxs-lookup"><span data-stu-id="d1295-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="d1295-109">**Μπορείτε να χρησιμοποιήσετε τη δυνατότητα της αίτησης πρόσβασης**</span><span class="sxs-lookup"><span data-stu-id="d1295-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="d1295-110">Η [δυνατότητα αίτησης πρόσβασης](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) επιτρέπει στους χρήστες να ζητούν πρόσβαση σε περιεχόμενο που δεν έχουν αυτήν τη στιγμή δικαίωμα να τις δείτε.</span><span class="sxs-lookup"><span data-stu-id="d1295-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="d1295-111">**Να επιτρέπεται η προσαρμοσμένη δέσμη ενεργειών ενδέχεται να προκαλέσει ζητήματα η πρόσβαση**</span><span class="sxs-lookup"><span data-stu-id="d1295-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="d1295-112">Υπάρχουν ορισμένα σενάρια όπου η δυνατότητα *προσαρμοσμένης δέσμης ενεργειών επιτρέπεται* μπορεί να παρουσιάσετε μια δεν επιτρέπεται η πρόσβαση.</span><span class="sxs-lookup"><span data-stu-id="d1295-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="d1295-113">Για μια λίστα με τις δυνατότητες που επηρεάζονται, ζητήματα ασφαλείας και για τη δυνατότητα να απενεργοποιήσετε τη δυνατότητα.</span><span class="sxs-lookup"><span data-stu-id="d1295-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="d1295-114">Επισκεφθείτε [επιτρέπεται ή να απαγορεύεται η προσαρμοσμένη δέσμη ενεργειών](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="d1295-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

