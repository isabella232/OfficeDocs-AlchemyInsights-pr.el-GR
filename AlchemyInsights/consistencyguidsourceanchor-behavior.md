---
title: Συμπεριφορά ConsistencyGuid /sourceAnchor
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
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: eafe1ec9636cddc9d73a88beb7ae3ad9f6fad660
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816992"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="3b0a7-102">Συμπεριφορά ConsistencyGuid /sourceAnchor</span><span class="sxs-lookup"><span data-stu-id="3b0a7-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="3b0a7-103">Το Azure AD Connect (έκδοση 1.1.524.0 και μετά) διευκολύνει πλέον τη χρήση του msDS-ConsistencyGuid ως χαρακτηριστικού sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="3b0a7-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="3b0a7-104">Κατά τη χρήση αυτής της δυνατότητας, το Azure AD Connect ρυθμίζει αυτόματα τις παραμέτρους των κανόνων συγχρονισμού ώστε:</span><span class="sxs-lookup"><span data-stu-id="3b0a7-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="3b0a7-105">Χρησιμοποιήστε το msDS-ConsistencyGuid ως το χαρακτηριστικό sourceAnchor για αντικείμενα χρήστη.</span><span class="sxs-lookup"><span data-stu-id="3b0a7-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="3b0a7-106">Το ObjectGUID χρησιμοποιείται για άλλους τύπους αντικειμένων.</span><span class="sxs-lookup"><span data-stu-id="3b0a7-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="3b0a7-107">Για οποιοδήποτε δεδομένο αντικείμενο χρήστη AD εσωτερικής εγκατάστασης του οποίου το χαρακτηριστικό msDS-ConsistencyGuid δεν έχει συμπληρωθεί, το Azure AD Connect επιστρέφει την τιμή objectGUID στο χαρακτηριστικό msDS-ConsistencyGuid στην υπηρεσία καταλόγου Active Directory εσωτερικής εγκατάστασης.</span><span class="sxs-lookup"><span data-stu-id="3b0a7-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="3b0a7-108">Μετά τη συμπλήρωση του χαρακτηριστικού msDS-ConsistencyGuid, το Azure AD Connect εξάγει το αντικείμενο στο Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3b0a7-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="3b0a7-109">**Σημείωση:** Μετά την εισαγωγή ενός αντικειμένου AD εσωτερικής εγκατάστασης στο Azure AD Connect (δηλαδή, εισάγεται στο χώρο σύνδεσης AD και προ βλάφεται στο Μετα-στίχο), δεν μπορείτε πλέον να αλλάξετε την τιμή sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="3b0a7-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="3b0a7-110">Για να καθορίσετε την τιμή sourceAnchor για ένα δεδομένο αντικείμενο AD εσωτερικής εγκατάστασης, ρυθμίστε τις παραμέτρους του χαρακτηριστικού msDS-ConsistencyGuid πριν από την εισαγωγή του στο Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="3b0a7-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="3b0a7-111">Για περισσότερες πληροφορίες σχετικά με το SourceAnchor και το ConsistencyGuid, ανατρέξτε στα εξής: [Azure AD Connect: Έννοιες σχεδίασης](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="3b0a7-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

