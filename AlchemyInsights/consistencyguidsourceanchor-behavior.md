---
title: Συμπεριφορά ConsistencyGuid/sourceAnchor
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: adac469328485696d1ee1532aa3d6828af0642eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47756283"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="13f59-102">Συμπεριφορά ConsistencyGuid/sourceAnchor</span><span class="sxs-lookup"><span data-stu-id="13f59-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="13f59-103">Το Azure AD Connect (έκδοση 1.1.524.0 και After) διευκολύνει πλέον τη χρήση των ΜΣΠ-ConsistencyGuid ως χαρακτηριστικό sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="13f59-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="13f59-104">Όταν χρησιμοποιείτε αυτήν τη δυνατότητα, το Azure AD Connect ρυθμίζει αυτόματα τους κανόνες συγχρονισμού σε:</span><span class="sxs-lookup"><span data-stu-id="13f59-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="13f59-105">Χρησιμοποιήστε τις ΜΣΠ-ConsistencyGuid ως το χαρακτηριστικό sourceAnchor για αντικείμενα χρήστη.</span><span class="sxs-lookup"><span data-stu-id="13f59-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="13f59-106">Το ObjectGUID χρησιμοποιείται για άλλους τύπους αντικειμένων.</span><span class="sxs-lookup"><span data-stu-id="13f59-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="13f59-107">Για οποιοδήποτε συγκεκριμένο αντικείμενο AD εσωτερικής εγκατάστασης του οποίου το χαρακτηριστικό ΜΣΠ-ConsistencyGuid δεν είναι συμπληρωμένο, το Azure AD Connect καταγράφει την τιμή του objectGUID στο χαρακτηριστικό ΜΣΠ-ConsistencyGuid στην υπηρεσία καταλόγου Active Directory εσωτερικής εγκατάστασης.</span><span class="sxs-lookup"><span data-stu-id="13f59-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="13f59-108">Μετά την συμπλήρωση του χαρακτηριστικού ΜΣΠ-ConsistencyGuid, το Azure AD Connect, στη συνέχεια, εξάγει το αντικείμενο στο Azure AD.</span><span class="sxs-lookup"><span data-stu-id="13f59-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="13f59-109">**Σημείωση:** Μόλις εισαχθεί ένα αντικείμενο AD εσωτερικής εγκατάστασης στο Azure AD Connect (δηλαδή, έχει εισαχθεί στον χώρο σύνδεσης AD και προβληθεί στην Metaverse), δεν μπορείτε πλέον να αλλάξετε την τιμή του sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="13f59-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="13f59-110">Για να καθορίσετε την τιμή sourceAnchor για ένα συγκεκριμένο αντικείμενο AD εσωτερικής εγκατάστασης, ρυθμίστε τις παραμέτρους του χαρακτηριστικού ΜΣΠ-ConsistencyGuid πριν από την εισαγωγή του στο Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="13f59-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="13f59-111">Για περισσότερες πληροφορίες σχετικά με το SourceAnchor και το ConsistencyGuid, ανατρέξτε στα εξής: [Azure AD Connect: έννοιες σχεδίασης](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="13f59-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

