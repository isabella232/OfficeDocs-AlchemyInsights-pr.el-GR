---
title: ConsistencyGuid / sourceAnchor συμπεριφορά
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: cb1b50792b07a1b3b69607bf2f6824141a15922f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32408108"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="3377a-102">ConsistencyGuid / sourceAnchor συμπεριφορά</span><span class="sxs-lookup"><span data-stu-id="3377a-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="3377a-103">Σύνδεση AD Azure (έκδοση 1.1.524.0 και μετά) τώρα διευκολύνει τη χρήση msDS-ConsistencyGuid ως χαρακτηριστικό sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="3377a-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="3377a-104">Όταν χρησιμοποιείτε αυτήν τη δυνατότητα, σύνδεση AD Azure ρυθμίζει αυτόματα τις παραμέτρους των κανόνων συγχρονισμού για να:</span><span class="sxs-lookup"><span data-stu-id="3377a-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="3377a-105">Χρησιμοποιήστε msDS-ConsistencyGuid με το χαρακτηριστικό sourceAnchor για αντικείμενα χρήστη.</span><span class="sxs-lookup"><span data-stu-id="3377a-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="3377a-106">ObjectGUID χρησιμοποιείται για άλλους τύπους αντικειμένου.</span><span class="sxs-lookup"><span data-stu-id="3377a-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="3377a-107">Για οποιαδήποτε λόγω εσωτερικής εγκατάστασης χρήστη AD αντικείμενο του οποίου το χαρακτηριστικό msDS-ConsistencyGuid δεν είναι συμπληρωμένη, Azure AD σύνδεση εγγράφει την τιμή objectGUID πίσω στο χαρακτηριστικό msDS-ConsistencyGuid εσωτερικής εγκατάστασης υπηρεσίας καταλόγου Active Directory.</span><span class="sxs-lookup"><span data-stu-id="3377a-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="3377a-108">Αφού συμπληρωθεί το χαρακτηριστικό msDS-ConsistencyGuid, σύνδεση AD Azure εξάγει, στη συνέχεια, το αντικείμενο Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3377a-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="3377a-109">**Σημείωση:** Μία φορά μια ενδοεταιρική αντικείμενο AD εισάγεται στη σύνδεση AD Azure (δηλαδή, εισάγονται στο χώρο της σύνδεσης AD και πρόβλεψη σε το Metaverse), δεν μπορείτε να αλλάξετε την τιμή της sourceAnchor πλέον.</span><span class="sxs-lookup"><span data-stu-id="3377a-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="3377a-110">Για να καθορίσετε την τιμή sourceAnchor για μια λόγω εσωτερικής εγκατάστασης AD αντικειμένων, να ρυθμίσετε τις παραμέτρους του χαρακτηριστικού msDS-ConsistencyGuid, πριν από την εισαγωγή σε σύνδεση AD Azure.</span><span class="sxs-lookup"><span data-stu-id="3377a-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="3377a-111">Για περισσότερες πληροφορίες σχετικά με SourceAnchor και ConsistencyGuid, ανατρέξτε στα παρακάτω: [σύνδεση AD Azure: Σχεδίαση έννοιες](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="3377a-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

