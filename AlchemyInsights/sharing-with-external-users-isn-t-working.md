---
title: Κοινή χρήση με εξωτερικούς χρήστες δεν λειτουργεί
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 69e290e5a13f40ad045086791189a7d0af88240b
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32369498"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="34201-102">Επιδιόρθωση προβλημάτων, κοινή χρήση περιεχομένου SharePoint με εξωτερικούς χρήστες</span><span class="sxs-lookup"><span data-stu-id="34201-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="34201-103">Βεβαιωθείτε ότι η εξωτερική κοινή χρήση είναι ενεργοποιημένη για την εταιρεία σας:</span><span class="sxs-lookup"><span data-stu-id="34201-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="34201-104">Μεταβείτε το [υπηρεσίες &amp; σελίδα προσθέτων στο Κέντρο διαχείρισης Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), και κάντε κλικ στο κουμπί **τοποθεσίες**.</span><span class="sxs-lookup"><span data-stu-id="34201-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="34201-105">Βεβαιωθείτε ότι η ρύθμιση είναι ενεργοποιημένη σε "Ενεργή".</span><span class="sxs-lookup"><span data-stu-id="34201-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="34201-106">Εάν έχει επιλεγεί "Μόνο υπάρχοντες χρήστες εξωτερικό", βεβαιωθείτε ότι το εξωτερικό χρήστη έχει καταχωρηθεί στο Κέντρο διαχείρισης Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="34201-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="34201-107">Βεβαιωθείτε ότι το εξωτερικό την κοινή χρήση του ενεργοποιημένο για την τοποθεσία.</span><span class="sxs-lookup"><span data-stu-id="34201-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="34201-108">Για μια συλλογή τοποθεσιών κλασική:</span><span class="sxs-lookup"><span data-stu-id="34201-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="34201-109">Με το νέο κέντρο διαχείρισης του SharePoint, στο αριστερό τμήμα του παραθύρου, κάντε κλικ στο κουμπί **τοποθεσίες**.</span><span class="sxs-lookup"><span data-stu-id="34201-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="34201-110">Επιλέξτε την τοποθεσία ή τοποθεσίες και, στην κορδέλα, κάντε κλικ στην εντολή **κοινή χρήση**.</span><span class="sxs-lookup"><span data-stu-id="34201-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="34201-111">Για μια τοποθεσία ομάδας που ανήκει σε μια ομάδα του Office 365 ή μια τοποθεσία επικοινωνίας:</span><span class="sxs-lookup"><span data-stu-id="34201-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="34201-112">Αυτοί οι τύποι νέα τοποθεσία έχουν το ίδιο κοινής χρήσης ρύθμιση ως τη ρύθμιση όλη την εταιρεία, εκτός εάν η ρύθμιση εταιρικά επιτρέπει την κοινή χρήση αρχείων, χρησιμοποιώντας τις συνδέσεις που δεν απαιτούν εισόδου.</span><span class="sxs-lookup"><span data-stu-id="34201-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="34201-113">Σε αυτήν την περίπτωση, τις τοποθεσίες επιτρέπουν την κοινή χρήση με νέους και υπάρχοντες εξωτερικούς χρήστες που θα εισέλθετε.</span><span class="sxs-lookup"><span data-stu-id="34201-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="34201-114">Για να αλλάξετε τη ρύθμιση για συγκεκριμένες τοποθεσίες, χρησιμοποιήστε το νέο κέντρο διαχείρισης του SharePoint ή PowerShell.</span><span class="sxs-lookup"><span data-stu-id="34201-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="34201-115">[Μάθετε περισσότερα](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="34201-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="34201-116">Η εξωτερική ρύθμιση κοινής χρήσης για κάθε τοποθεσία μπορεί να είναι πιο περιοριστικές από τη ρύθμιση όλη την εταιρεία, αλλά δεν είναι πλέον προαιρετικές από τη ρύθμιση όλον τον οργανισμό.</span><span class="sxs-lookup"><span data-stu-id="34201-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

