---
title: Προβλήματα επιδόσεων-SharePoint ή OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 39ec9b746c47414f1cfaad1342491b8f33a47d6f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771244"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="025cb-102">Το SharePoint ή το OneDrive είναι αργά, απρόσιτα ή μη διαθέσιμα για πολλούς χρήστες</span><span class="sxs-lookup"><span data-stu-id="025cb-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="025cb-103">Εάν μια τοποθεσία του OneDrive ή του SharePoint δεν είναι διαθέσιμη για πολλούς χρήστες που είχαν προηγουμένως πρόσβαση, μπορεί να υπάρχει κάποιο πρόβλημα προσωρινής υπηρεσίας.</span><span class="sxs-lookup"><span data-stu-id="025cb-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="025cb-104">[Επιλέξτε τον πίνακα εργαλείων εύρυθμης λειτουργίας υπηρεσίας](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="025cb-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="025cb-105">**Προσθήκη και άδεια χρήσης του χρήστη**</span><span class="sxs-lookup"><span data-stu-id="025cb-105">**Add and license the user**</span></span>

<span data-ttu-id="025cb-106">Βεβαιωθείτε ότι [εκχωρείτε άδειες χρήσης σε χρήστες στο Microsoft 365 για επαγγελματικούς λόγους](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="025cb-106">Ensure that you [Assign licenses to users in Microsoft 365 for business](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span>


<span data-ttu-id="025cb-107">**Εκχώρηση δικαιωμάτων**</span><span class="sxs-lookup"><span data-stu-id="025cb-107">**Assign Permissions**</span></span>

<span data-ttu-id="025cb-108">Εάν ο χρήστης έχει εκχωρηθεί μια άδεια χρήσης του SharePoint και εξακολουθεί να λαμβάνει ένα μήνυμα που δεν επιτρέπεται η πρόσβαση, βεβαιωθείτε ότι έχει εκχωρηθεί το [κατάλληλο επίπεδο δικαιωμάτων](https://docs.microsoft.com/sharepoint/understanding-permission-levels) .</span><span class="sxs-lookup"><span data-stu-id="025cb-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="025cb-109">**Εξετάστε το ενδεχόμενο χρήσης της δυνατότητας αίτησης πρόσβασης**</span><span class="sxs-lookup"><span data-stu-id="025cb-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="025cb-110">Η [δυνατότητα αίτησης πρόσβασης](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) επιτρέπει στους χρήστες να ζητούν πρόσβαση σε περιεχόμενο που δεν έχουν προς το παρόν δικαίωμα να βλέπουν.</span><span class="sxs-lookup"><span data-stu-id="025cb-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="025cb-111">**Η προσαρμοσμένη δέσμη ενεργειών μπορεί να προκαλέσει προβλήματα που δεν επιτρέπονται στην Access**</span><span class="sxs-lookup"><span data-stu-id="025cb-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="025cb-112">Υπάρχουν ορισμένα σενάρια όπου η δυνατότητα "να *επιτρέπεται η προσαρμοσμένη δέσμη ενεργειών* " μπορεί να παρουσιάζει άρνηση πρόσβασης.</span><span class="sxs-lookup"><span data-stu-id="025cb-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="025cb-113">Για μια λίστα με τις δυνατότητες που επηρεάζονται, θέματα ασφαλείας και τη δυνατότητα να απενεργοποιήσετε τη δυνατότητα.</span><span class="sxs-lookup"><span data-stu-id="025cb-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="025cb-114">Παρακαλούμε επισκεφθείτε την επιλογή [Αποδοχή ή αποτροπή προσαρμοσμένης δέσμης ενεργειών](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="025cb-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

