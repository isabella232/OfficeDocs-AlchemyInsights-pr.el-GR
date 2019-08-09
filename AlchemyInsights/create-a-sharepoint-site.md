---
title: Δημιουργία μιας τοποθεσίας του SharePoint
ms.author: efrene
author: efrene
ms.date: 1/16/2019
ms.audience: ITPro
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: ad1a77b69d2d453dbd3daa304759238b329f96ba
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/09/2019
ms.locfileid: "36269916"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="46c5e-102">Δημιουργία μιας τοποθεσίας του SharePoint</span><span class="sxs-lookup"><span data-stu-id="46c5e-102">Create a SharePoint site</span></span>

<span data-ttu-id="46c5e-103">Μπορείτε να δείτε τα ακόλουθα, για πληροφορίες σχετικά με τη δημιουργία τοποθεσίας του SharePoint:</span><span class="sxs-lookup"><span data-stu-id="46c5e-103">You can see the following for information about SharePoint site creation:</span></span>
- <span data-ttu-id="46c5e-104">[Διαχείριση τοποθεσιών στο νέο κέντρο διαχείρισης του SharePoint](https://docs.microsoft.com/sharepoint/manage-site-creation): Μάθετε σχετικά με τις επιλογές δημιουργίας τοποθεσίας, καθώς και τον τρόπο δημιουργίας μια κλασική τοποθεσία ή μια τοποθεσία ομάδες που δεν περιλαμβάνει μια ομάδα Office 365.</span><span class="sxs-lookup"><span data-stu-id="46c5e-104">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation): Learn about site creation options, including how to create a classic site or a teams site that doesn't include an Office 365 group.</span></span>
- <span data-ttu-id="46c5e-105">[Δημιουργία τοποθεσίας ομάδας του SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US): Μάθετε πώς μπορείτε να δημιουργήσετε μια τοποθεσία ομάδας.</span><span class="sxs-lookup"><span data-stu-id="46c5e-105">[Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US): Learn how to create a team site.</span></span>
- <span data-ttu-id="46c5e-106">[Δημιουργία τοποθεσίας στο SharePoint ηλεκτρονική επικοινωνία](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Μάθετε πώς μπορείτε να δημιουργήσετε μια τοποθεσία επικοινωνίας.</span><span class="sxs-lookup"><span data-stu-id="46c5e-106">[Create a communication site in SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Learn how to create a communications site.</span></span>
- <span data-ttu-id="46c5e-107">[Διαχείριση τοποθεσιών στο νέο κέντρο διαχείρισης του SharePoint](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site): Μάθετε πώς να δημιουργείτε μια κλασική τοποθεσία ή μια τοποθεσία ομάδας που δεν περιλαμβάνει μια ομάδα Office 365.</span><span class="sxs-lookup"><span data-stu-id="46c5e-107">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site):  Learn how to create a classic site or a team site that doesn't include an Office 365 group.</span></span>


  
> [! Συμβουλές]
> - <span data-ttu-id="46c5e-109">Δεν μπορείτε να δημιουργήσετε μια τοποθεσία με την ίδια διεύθυνση URL μιας υπάρχουσας τοποθεσίας.</span><span class="sxs-lookup"><span data-stu-id="46c5e-109">You cannot create a site with the same URL of an existing site.</span></span> <span data-ttu-id="46c5e-110">Εάν διαγράψετε μια τοποθεσία και που επιθυμεί να χρησιμοποιήσει ξανά τη διεύθυνση URL, είναι δυνατή τη διαγραμμένη τοποθεσία εξακολουθεί να υπάρχει στην περιοχή **τοποθεσιών διαγράφηκε**.</span><span class="sxs-lookup"><span data-stu-id="46c5e-110">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**.</span></span> <span data-ttu-id="46c5e-111">Για να διαχειριστείτε διαγραφή δείτε τοποθεσίες, [Διαγραφή μιας τοποθεσίας](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="46c5e-111">To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span></span> <span data-ttu-id="46c5e-112">Για να καταργήσετε πλήρως μια τοποθεσία με Powershell, δείτε το παράδειγμα cmdlet [Remove SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) .</span><span class="sxs-lookup"><span data-stu-id="46c5e-112">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
> - <span data-ttu-id="46c5e-113">Κάποιοι χρήστες ενδέχεται να μην έχετε τη δυνατότητα να δημιουργήσετε μια τοποθεσία.</span><span class="sxs-lookup"><span data-stu-id="46c5e-113">Some users may not be able to create a site.</span></span> <span data-ttu-id="46c5e-114">Ανατρέξτε στην ενότητα [Διαχείριση δημιουργίας τοποθεσίας στο SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="46c5e-114">See [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
> - <span data-ttu-id="46c5e-115">Είναι πιθανό η τοποθεσία φαίνεται να έχει μπλοκάρει σε **Δημιουργία** περισσότερο από το αναμενόμενο.</span><span class="sxs-lookup"><span data-stu-id="46c5e-115">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="46c5e-116">Εάν έχουν περάσει περισσότερες από 24 ώρες, από τη στιγμή που είδατε πρώτα αυτό το ζήτημα, συνδεθείτε ένα εισιτήριο υποστήριξης.</span><span class="sxs-lookup"><span data-stu-id="46c5e-116">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="46c5e-117">Σε πολλές περιπτώσεις, εργαζόμαστε ήδη σε μια λύση.</span><span class="sxs-lookup"><span data-stu-id="46c5e-117">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="46c5e-118">Παρακαλούμε να μας δώσετε τουλάχιστον 24 ώρες για να ολοκληρωθεί μια λύση.</span><span class="sxs-lookup"><span data-stu-id="46c5e-118">Please give us at least 24 hours to complete a solution.</span></span>
> - <span data-ttu-id="46c5e-119">Εάν θέλετε να δημιουργήσετε μια νέα τοποθεσία ομάδας που δεν περιλαμβάνει μια ομάδα Office 365,</span><span class="sxs-lookup"><span data-stu-id="46c5e-119">If you need to create a new team site that doesn't include an Office 365 group,</span></span> 


