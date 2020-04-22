---
title: Ζητήματα επιδόσεων-SharePoint ή OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: ec378981d4f24837b037e18214cbeba2f2b657c5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692693"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="b7282-102">SharePoint ή OneDrive αργή, απρόσιτη ή μη διαθέσιμη για πολλούς χρήστες</span><span class="sxs-lookup"><span data-stu-id="b7282-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="b7282-103">Εάν μια τοποθεσία του OneDrive ή του SharePoint δεν είναι διαθέσιμη σε πολλούς χρήστες που είχαν προηγουμένως πρόσβαση, ενδέχεται να υπάρχει ένα ζήτημα προσωρινής υπηρεσίας.</span><span class="sxs-lookup"><span data-stu-id="b7282-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="b7282-104">[Ελέγξτε τον πίνακα εργαλείων εύρυθμης λειτουργίας υπηρεσίας](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="b7282-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="b7282-105">**Προσθήκη και άδεια χρήσης του χρήστη**</span><span class="sxs-lookup"><span data-stu-id="b7282-105">**Add and license the user**</span></span>

<span data-ttu-id="b7282-106">Βεβαιωθείτε ότι [εκχωρείτε άδειες χρήσης σε χρήστες του Microsoft 365 για επιχειρήσεις](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="b7282-106">Ensure that you [Assign licenses to users in Microsoft 365 for business](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span>


<span data-ttu-id="b7282-107">**Εκχώρηση δικαιωμάτων**</span><span class="sxs-lookup"><span data-stu-id="b7282-107">**Assign Permissions**</span></span>

<span data-ttu-id="b7282-108">Εάν ο χρήστης έχει λάβει μια άδεια χρήσης του Sharepoint και εξακολουθεί να λαμβάνει ένα μήνυμα που δεν επιτρέπεται πρόσβασης, βεβαιωθείτε ότι έχει αντιστοιχιστεί το [κατάλληλο επίπεδο δικαιωμάτων.](https://docs.microsoft.com/sharepoint/understanding-permission-levels)</span><span class="sxs-lookup"><span data-stu-id="b7282-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="b7282-109">**Εξετάστε το ενδεχόμενο να χρησιμοποιήσετε τη δυνατότητα αίτησης πρόσβασης**</span><span class="sxs-lookup"><span data-stu-id="b7282-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="b7282-110">Η [δυνατότητα αίτησης πρόσβασης](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) επιτρέπει στους χρήστες να ζητούν πρόσβαση σε περιεχόμενο που δεν έχουν αυτήν τη στιγμή δικαίωμα προβολής.</span><span class="sxs-lookup"><span data-stu-id="b7282-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="b7282-111">**Να επιτρέπεται η προσαρμοσμένη δέσμη ενεργειών ενδέχεται να προκαλέσει ζητήματα άρνησης πρόσβασης**</span><span class="sxs-lookup"><span data-stu-id="b7282-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="b7282-112">Υπάρχουν ορισμένα σενάρια όπου η δυνατότητα *"Να επιτρέπεται η προσαρμοσμένη δέσμη ενεργειών"* ενδέχεται να παρουσιάζει μια πρόσβαση που δεν επιτρέπεται.</span><span class="sxs-lookup"><span data-stu-id="b7282-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="b7282-113">Για μια λίστα δυνατοτήτων που επηρεάζονται, ζητήματα ασφαλείας και τη δυνατότητα απενεργοποίησης της δυνατότητας.</span><span class="sxs-lookup"><span data-stu-id="b7282-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="b7282-114">Παρακαλώ επισκεφθείτε [Την επιλογή Να επιτρέπεται ή να μην επιτρέπεται η προσαρμοσμένη δέσμη ενεργειών](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="b7282-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

