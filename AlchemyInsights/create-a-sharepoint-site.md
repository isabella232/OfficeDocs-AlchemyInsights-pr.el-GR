---
title: Δημιουργία μιας τοποθεσίας του SharePoint
ms.author: kirks
author: Techwriter40
ms.date: 1/16/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1386"
- "2303"
- "5200004"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: cc0218dd34844cc1fdeb55a6f84975311826c372
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35364553"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="f34dc-102">Δημιουργία μιας τοποθεσίας του SharePoint</span><span class="sxs-lookup"><span data-stu-id="f34dc-102">Create a SharePoint site</span></span>

<span data-ttu-id="f34dc-103">Για επιλογές για τη δημιουργία τοποθεσιών, ανατρέξτε στην ενότητα [Διαχείριση τοποθεσιών στο νέο κέντρο διαχείρισης του SharePoint](https://docs.microsoft.com/sharepoint/manage-site-creation ) .</span><span class="sxs-lookup"><span data-stu-id="f34dc-103">See [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation ) for site creation options.</span></span> <span data-ttu-id="f34dc-104">Επιλέξτε για να δημιουργήσετε μια [τοποθεσία ομάδας](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US) (η οποία θα δημιουργήσει μια ομάδα Office 365) ή μια [τοποθεσία επικοινωνίας](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb).</span><span class="sxs-lookup"><span data-stu-id="f34dc-104">Select to create a [team site](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US) (which will create an Office 365 group) or a [communication site](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb).</span></span> <span data-ttu-id="f34dc-105">Για να δημιουργήσετε μια [κλασική τοποθεσίας](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site)ή μια νέα τοποθεσία ομάδας που δεν περιλαμβάνει μια ομάδα Office 365, κάντε κλικ στις **άλλες επιλογές**.</span><span class="sxs-lookup"><span data-stu-id="f34dc-105">To create a [classic site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site), or a new team site that doesn't include an Office 365 group, click **Other options**.</span></span>
  
<span data-ttu-id="f34dc-106">Συμβουλές:</span><span class="sxs-lookup"><span data-stu-id="f34dc-106">Tips:</span></span>
- <span data-ttu-id="f34dc-107">*Δεν μπορείτε να δημιουργήσετε μια τοποθεσία με την ίδια διεύθυνση URL μιας υπάρχουσας τοποθεσίας. Εάν διαγράψετε μια τοποθεσία και που επιθυμεί να χρησιμοποιήσει ξανά τη διεύθυνση URL, είναι δυνατή τη διαγραμμένη τοποθεσία εξακολουθεί να υπάρχει στην περιοχή **τοποθεσιών διαγράφηκε**. Για να διαχειριστείτε διαγραφή δείτε τοποθεσίες, [Διαγραφή μιας τοποθεσίας](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site). Για να καταργήσετε πλήρως μια τοποθεσία με Powershell, δείτε το παράδειγμα cmdlet [Remove SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) .*</span><span class="sxs-lookup"><span data-stu-id="f34dc-107">*You cannot create a site with the same URL of an existing site. If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**. To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site). To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.*</span></span>
- <span data-ttu-id="f34dc-108">*Κάποιοι χρήστες ενδέχεται να μην έχετε τη δυνατότητα να δημιουργήσετε μια τοποθεσία. Ανατρέξτε στην ενότητα [Διαχείριση δημιουργίας τοποθεσίας στο SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).*</span><span class="sxs-lookup"><span data-stu-id="f34dc-108">*Some users may not be able to create a site. See [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).*</span></span>
- <span data-ttu-id="f34dc-109">*Είναι πιθανό η τοποθεσία φαίνεται να έχει μπλοκάρει σε **Δημιουργία** περισσότερο από το αναμενόμενο. Εάν έχουν περάσει περισσότερες από 24 ώρες, από τη στιγμή που είδατε πρώτα αυτό το ζήτημα, συνδεθείτε ένα εισιτήριο υποστήριξης. Σε πολλές περιπτώσεις, εργαζόμαστε ήδη σε μια λύση. Παρακαλούμε να μας δώσετε τουλάχιστον 24 ώρες για να ολοκληρωθεί μια λύση.*</span><span class="sxs-lookup"><span data-stu-id="f34dc-109">*It's possible the site appears stuck at **Creating** longer than expected. If more than 24 hours have passed since you first saw this issue, please log a support ticket. In many cases, we're already working on a solution. Please give us at least 24 hours to complete a solution.*</span></span>
