---
title: Δημιουργία τοποθεσίας του SharePoint
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: 2611c3ed9cfe78c82c9b123ea26b6fe8f951b458
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049877"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="bd685-102">Δημιουργία τοποθεσίας του SharePoint</span><span class="sxs-lookup"><span data-stu-id="bd685-102">Create a SharePoint site</span></span>

<span data-ttu-id="bd685-103">Μπορείτε να δείτε τα παρακάτω για πληροφορίες σχετικά με τη δημιουργία τοποθεσίας SharePoint:</span><span class="sxs-lookup"><span data-stu-id="bd685-103">You can see the following for information about SharePoint site creation:</span></span>
- <span data-ttu-id="bd685-104">[Διαχείριση τοποθεσιών στο νέο κέντρο διαχείρισης του SharePoint](https://docs.microsoft.com/sharepoint/manage-site-creation): Μάθετε σχετικά με τις επιλογές δημιουργίας τοποθεσιών, συμπεριλαμβανομένου του τρόπου δημιουργίας μιας κλασικής τοποθεσίας ή μιας τοποθεσίας ομάδων που δεν περιλαμβάνει μια ομάδα Office 365.</span><span class="sxs-lookup"><span data-stu-id="bd685-104">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation): Learn about site creation options, including how to create a classic site or a teams site that doesn't include an Office 365 group.</span></span>
- <span data-ttu-id="bd685-105">[Δημιουργία μιας τοποθεσίας ομάδας στο SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d): Μάθετε πώς μπορείτε να δημιουργήσετε μια τοποθεσία ομάδας.</span><span class="sxs-lookup"><span data-stu-id="bd685-105">[Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d): Learn how to create a team site.</span></span>
- <span data-ttu-id="bd685-106">[Δημιουργήστε μια τοποθεσία επικοινωνίας στο SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Μάθετε πώς μπορείτε να δημιουργήσετε μια τοποθεσία επικοινωνιών.</span><span class="sxs-lookup"><span data-stu-id="bd685-106">[Create a communication site in SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Learn how to create a communications site.</span></span>
- <span data-ttu-id="bd685-107">[Διαχείριση τοποθεσιών στο νέο κέντρο διαχείρισης του SharePoint](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site): Μάθετε πώς μπορείτε να δημιουργήσετε μια κλασική τοποθεσία ή μια τοποθεσία ομάδας που δεν περιλαμβάνει μια ομάδα Office 365.</span><span class="sxs-lookup"><span data-stu-id="bd685-107">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site):  Learn how to create a classic site or a team site that doesn't include an Office 365 group.</span></span>


  
<span data-ttu-id="bd685-108">**Συμβουλές:**</span><span class="sxs-lookup"><span data-stu-id="bd685-108">**Tips:**</span></span>
- <span data-ttu-id="bd685-109">Δεν μπορείτε να δημιουργήσετε μια τοποθεσία με την ίδια διεύθυνση URL μιας υπάρχουσας τοποθεσίας.</span><span class="sxs-lookup"><span data-stu-id="bd685-109">You cannot create a site with the same URL of an existing site.</span></span> <span data-ttu-id="bd685-110">Εάν διαγράψατε μια τοποθεσία και επιθυμείτε να χρησιμοποιήσετε ξανά τη διεύθυνση URL, είναι πιθανό η διαγραμμένη τοποθεσία να εξακολουθεί να υπάρχει κάτω από τις **διαγραμμένες τοποθεσίες**.</span><span class="sxs-lookup"><span data-stu-id="bd685-110">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**.</span></span> <span data-ttu-id="bd685-111">Για να διαχειριστείτε τις διαγραμμένες τοποθεσίες, δείτε, [Διαγράψτε μια τοποθεσία](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="bd685-111">To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span></span> <span data-ttu-id="bd685-112">Για να καταργήσετε εντελώς μια τοποθεσία με PowerShell, δείτε το παράδειγμα cmdlet [Κατάργηση SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) .</span><span class="sxs-lookup"><span data-stu-id="bd685-112">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="bd685-113">Ορισμένοι χρήστες ενδέχεται να μην είναι σε θέση να δημιουργήσουν μια τοποθεσία.</span><span class="sxs-lookup"><span data-stu-id="bd685-113">Some users may not be able to create a site.</span></span> <span data-ttu-id="bd685-114">Ανατρέξτε [στην περιοχή Διαχείριση δημιουργίας τοποθεσίας στο SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="bd685-114">See [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="bd685-115">Είναι πιθανό ο ιστότοπος να εμφανίζεται κολλημένος στη **Δημιουργία** μεγαλύτερου από το αναμενόμενο.</span><span class="sxs-lookup"><span data-stu-id="bd685-115">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="bd685-116">Εάν έχουν περάσει περισσότερες από 24 ώρες από τότε που είδατε για πρώτη φορά αυτό το ζήτημα, παρακαλούμε να καταγράψετε ένα εισιτήριο υποστήριξης.</span><span class="sxs-lookup"><span data-stu-id="bd685-116">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="bd685-117">Σε πολλές περιπτώσεις, ήδη εργαζόμαστε για μια λύση.</span><span class="sxs-lookup"><span data-stu-id="bd685-117">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="bd685-118">Παρακαλώ δώστε μας τουλάχιστον 24 ώρες για να ολοκληρώσουμε μια λύση.</span><span class="sxs-lookup"><span data-stu-id="bd685-118">Please give us at least 24 hours to complete a solution.</span></span>
- <span data-ttu-id="bd685-119">Εάν χρειάζεται να δημιουργήσετε μια νέα τοποθεσία ομάδας που δεν περιλαμβάνει μια ομάδα Office 365,</span><span class="sxs-lookup"><span data-stu-id="bd685-119">If you need to create a new team site that doesn't include an Office 365 group,</span></span> 


