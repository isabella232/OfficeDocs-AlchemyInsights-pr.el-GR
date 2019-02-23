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
ms.custom: Adm_O365
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 4b132a3cb0fac015ab44a1fa08565af15b7e8121
ms.sourcegitcommit: c003a5db7edc3a44fb5b31b46cd45f12b62d172a
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 02/22/2019
ms.locfileid: "30207685"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="94cf9-102">Επιδιόρθωση προβλημάτων, κοινή χρήση περιεχομένου SharePoint με εξωτερικούς χρήστες</span><span class="sxs-lookup"><span data-stu-id="94cf9-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="94cf9-103">Βεβαιωθείτε ότι η εξωτερική κοινή χρήση είναι ενεργοποιημένη για την εταιρεία σας:</span><span class="sxs-lookup"><span data-stu-id="94cf9-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="94cf9-104">Μεταβείτε το [υπηρεσίες &amp; σελίδα προσθέτων στο Κέντρο διαχείρισης Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), και κάντε κλικ στο κουμπί **τοποθεσίες**.</span><span class="sxs-lookup"><span data-stu-id="94cf9-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="94cf9-p101">Βεβαιωθείτε ότι η ρύθμιση είναι ενεργοποιημένη σε "Ενεργή". Εάν έχει επιλεγεί "Μόνο υπάρχοντες χρήστες εξωτερικό", βεβαιωθείτε ότι το εξωτερικό χρήστη έχει καταχωρηθεί στο Κέντρο διαχείρισης Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="94cf9-p101">Make sure the setting is turned to "On." If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="94cf9-p102">Βεβαιωθείτε ότι το εξωτερικό την κοινή χρήση του ενεργοποιημένο για την τοποθεσία. Για μια συλλογή τοποθεσιών κλασική:</span><span class="sxs-lookup"><span data-stu-id="94cf9-p102">Make sure external sharing it turned on for the site. For a classic site collection:</span></span>
  
1. <span data-ttu-id="94cf9-109">Στο κλασικό στο Κέντρο διαχείρισης του SharePoint, στο αριστερό τμήμα του παραθύρου, κάντε κλικ στην επιλογή **συλλογές τοποθεσιών**.</span><span class="sxs-lookup"><span data-stu-id="94cf9-109">In the classic SharePoint admin center, in the left pane, click **site collections**.</span></span>
    
2. <span data-ttu-id="94cf9-110">Επιλέξτε την τοποθεσία ή τοποθεσίες και, στην κορδέλα, κάντε κλικ στην εντολή **κοινή χρήση**.</span><span class="sxs-lookup"><span data-stu-id="94cf9-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="94cf9-111">Για μια τοποθεσία ομάδας που ανήκει σε μια ομάδα του Office 365 ή μια τοποθεσία επικοινωνίας:</span><span class="sxs-lookup"><span data-stu-id="94cf9-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="94cf9-p103">Αυτοί οι τύποι νέα τοποθεσία έχουν το ίδιο κοινής χρήσης ρύθμιση ως τη ρύθμιση όλη την εταιρεία, εκτός εάν η ρύθμιση εταιρικά επιτρέπει την κοινή χρήση αρχείων, χρησιμοποιώντας τις συνδέσεις που δεν απαιτούν εισόδου. Σε αυτήν την περίπτωση, τις τοποθεσίες επιτρέπουν την κοινή χρήση με νέους και υπάρχοντες εξωτερικούς χρήστες που θα εισέλθετε. Για να αλλάξετε τη ρύθμιση για συγκεκριμένες τοποθεσίες, χρησιμοποιήστε το νέο κέντρο διαχείρισης του SharePoint (προεπισκόπηση) ή PowerShell. [Μάθετε περισσότερα](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="94cf9-p103">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in. In this case, the sites allow sharing with new and existing external users who sign in. To change the setting for specific sites, use the new SharePoint admin center (preview) or PowerShell. [Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="94cf9-116">Η εξωτερική ρύθμιση κοινής χρήσης για κάθε τοποθεσία μπορεί να είναι πιο περιοριστικές από τη ρύθμιση όλη την εταιρεία, αλλά δεν είναι πλέον προαιρετικές από τη ρύθμιση όλον τον οργανισμό.</span><span class="sxs-lookup"><span data-stu-id="94cf9-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

