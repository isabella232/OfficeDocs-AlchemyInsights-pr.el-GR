---
title: Ζητήματα επιδόσεων-SharePoint ή OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 7e218cfff81274cd16d55dec2c5243eb8b74a3b7
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 10/18/2019
ms.locfileid: "36750556"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="f2a3f-102">Το SharePoint ή το OneDrive αργή, μη προσβάσιμη ή μη διαθέσιμη για πολλαπλούς χρήστες</span><span class="sxs-lookup"><span data-stu-id="f2a3f-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="f2a3f-103">Εάν μια τοποθεσία OneDrive ή SharePoint δεν είναι διαθέσιμη σε πολλούς χρήστες που είχαν προηγουμένως πρόσβαση, ενδέχεται να υπάρχει ένα ζήτημα προσωρινής υπηρεσίας.</span><span class="sxs-lookup"><span data-stu-id="f2a3f-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="f2a3f-104">[Ελέγξτε τον πίνακα εργαλείων εύρυθμης λειτουργίας υπηρεσίας](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="f2a3f-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="f2a3f-105">**Προσθήκη και άδεια χρήσης του χρήστη**</span><span class="sxs-lookup"><span data-stu-id="f2a3f-105">**Add and license the user**</span></span>

<span data-ttu-id="f2a3f-106">Βεβαιωθείτε ότι [εκχωρείτε άδειες χρήσης σε χρήστες του Office 365 για επιχειρήσεις](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="f2a3f-106">Ensure that you [Assign licenses to users in Office 365 for business](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span>


<span data-ttu-id="f2a3f-107">**Εκχώρηση δικαιωμάτων**</span><span class="sxs-lookup"><span data-stu-id="f2a3f-107">**Assign Permissions**</span></span>

<span data-ttu-id="f2a3f-108">Εάν ο χρήστης έχει εκχωρηθεί μια άδεια χρήσης του SharePoint και εξακολουθεί να λαμβάνει ένα μήνυμα άρνησης πρόσβασης, βεβαιωθείτε ότι έχουν εκχωρηθεί το [κατάλληλο επίπεδο δικαιωμάτων](https://docs.microsoft.com/sharepoint/understanding-permission-levels) .</span><span class="sxs-lookup"><span data-stu-id="f2a3f-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="f2a3f-109">**Εξετάστε το ενδεχόμενο να χρησιμοποιήσετε τη δυνατότητα αίτησης πρόσβασης**</span><span class="sxs-lookup"><span data-stu-id="f2a3f-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="f2a3f-110">Η [δυνατότητα αίτησης πρόσβασης](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) επιτρέπει στους χρήστες να ζητήσουν πρόσβαση σε περιεχόμενο που δεν έχουν αυτήν τη στιγμή δικαίωμα να δουν.</span><span class="sxs-lookup"><span data-stu-id="f2a3f-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="f2a3f-111">**Να επιτρέπεται η προσαρμοσμένη δέσμη ενεργειών μπορεί να προκαλέσει ζητήματα άρνησης πρόσβασης**</span><span class="sxs-lookup"><span data-stu-id="f2a3f-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="f2a3f-112">Υπάρχουν ορισμένα σενάρια όπου η δυνατότητα *προσαρμοσμένης δέσμης ενεργειών* μπορεί να παρουσιάζει μια πρόσβαση δεν επιτρέπεται.</span><span class="sxs-lookup"><span data-stu-id="f2a3f-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="f2a3f-113">Για μια λίστα με τις δυνατότητες που επηρεάζονται, ζητήματα ασφαλείας και τη δυνατότητα απενεργοποίησης της δυνατότητας.</span><span class="sxs-lookup"><span data-stu-id="f2a3f-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="f2a3f-114">Παρακαλούμε επισκεφθείτε την [Αποδοχή ή την αποτροπή προσαρμοσμένης δέσμης ενεργειών](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="f2a3f-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

