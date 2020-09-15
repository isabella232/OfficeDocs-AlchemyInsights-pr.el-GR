---
title: Εκχώρηση πρόσβασης στους χρήστες στο SharePoint και το OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: a7e9c0b7ffa5c11a2e24ee5fda6491f049f985f1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677207"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a><span data-ttu-id="c2091-102">Εκχώρηση πρόσβασης στους χρήστες στο SharePoint και το OneDrive</span><span class="sxs-lookup"><span data-stu-id="c2091-102">Give users access to SharePoint and OneDrive</span></span>

> [!NOTE]
> <span data-ttu-id="c2091-103">Εάν μια τοποθεσία του OneDrive ή του SharePoint δεν είναι διαθέσιμη για πολλούς χρήστες που είχαν προηγουμένως πρόσβαση, μπορεί να υπάρχει κάποιο πρόβλημα προσωρινής υπηρεσίας.</span><span class="sxs-lookup"><span data-stu-id="c2091-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> [<span data-ttu-id="c2091-104">Επιλέξτε τον πίνακα εργαλείων εύρυθμης λειτουργίας υπηρεσίας</span><span class="sxs-lookup"><span data-stu-id="c2091-104">Check the service health dashboard</span></span>](https://portal.office.com/adminportal/home#/servicehealth)
  
<span data-ttu-id="c2091-105">Εάν θέλετε τα άτομα στην εταιρεία σας να έχουν τη δυνατότητα εισόδου και χρήσης του SharePoint και του OneDrive, πρέπει να προσθέσετε λογαριασμούς για αυτούς και να βεβαιωθείτε ότι έχουν μια άδεια χρήσης που τους παρέχει πρόσβαση στο SharePoint και το OneDrive.</span><span class="sxs-lookup"><span data-stu-id="c2091-105">If you want people in your organization to be able to sign in and use SharePoint and OneDrive, you need to add accounts for them and make sure they have a license that gives them access to SharePoint and OneDrive.</span></span> <span data-ttu-id="c2091-106">Ο ευκολότερος τρόπος για να προσθέσετε χρήστες είναι το κέντρο διαχείρισης του Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="c2091-106">The easiest way to add users is in the Microsoft 365 admin center.</span></span>
  
1. <span data-ttu-id="c2091-107">Μεταβείτε στη [σελίδα "ενεργοί χρήστες" στο κέντρο διαχείρισης του Microsoft 365](https://portal.office.com/adminportal/home#/users)και, στη συνέχεια, κάντε κλικ στην επιλογή **Προσθήκη χρήστη**.</span><span class="sxs-lookup"><span data-stu-id="c2091-107">Go to the [Active users page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/users), and then click **Add a user**.</span></span>
    
2. <span data-ttu-id="c2091-108">Συμπληρώστε τις πληροφορίες για το χρήστη και βεβαιωθείτε ότι, στην περιοχή **άδειες χρήσης προϊόντος**, έχει εκχωρηθεί μια άδεια χρήσης και είναι επιλεγμένο το **SharePoint Online** .</span><span class="sxs-lookup"><span data-stu-id="c2091-108">Fill in the information for the user, and make sure that under **Product licenses**, a license is assigned and **SharePoint Online** is selected.</span></span> 
    
<span data-ttu-id="c2091-109">Λάβετε υπόψη ότι εάν επιτρέψετε την εξωτερική κοινή χρήση στην εταιρεία σας, οι χρήστες μπορούν να κάνουν κοινή χρήση περιεχομένου του SharePoint και του OneDrive με άτομα εκτός του οργανισμού.</span><span class="sxs-lookup"><span data-stu-id="c2091-109">Note that if you allow external sharing in your organization, users can share SharePoint and OneDrive content with people outside the organization.</span></span> <span data-ttu-id="c2091-110">Δεν χρειάζεται να παράσχετε άδειες χρήσης σε αυτούς τους εξωτερικούς χρήστες.</span><span class="sxs-lookup"><span data-stu-id="c2091-110">You don't need to give these external users licenses.</span></span> <span data-ttu-id="c2091-111">Επίσης, δεν χρειάζεται να προσθέσετε λογαριασμούς για αυτούς, εκτός εάν η κοινή χρήση έχει καθοριστεί σε "μόνο οι υπάρχοντες εξωτερικοί χρήστες".</span><span class="sxs-lookup"><span data-stu-id="c2091-111">You also don't need to add accounts for them, unless sharing is set to "Only existing external users."</span></span> <span data-ttu-id="c2091-112">Σε αυτή την περίπτωση, εάν τα άτομα δεν βρίσκονται στον κατάλογο της εταιρείας σας, πρέπει να τα προσθέσετε ως χρήστες Guest στο κέντρο διαχείρισης Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c2091-112">In that case, if the people aren't in your organization's directory, you need to add them as guest users in the Azure AD admin center.</span></span>
  

