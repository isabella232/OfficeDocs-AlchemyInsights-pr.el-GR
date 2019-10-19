---
title: Συμπεριφορά αγκύρωσης/προέλευσης
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
ms.openlocfilehash: f0ff94a8e46f1fb4e0ac8653c51f8f651e29498b
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 10/18/2019
ms.locfileid: "36516981"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="fcc5d-102">Συμπεριφορά αγκύρωσης/προέλευσης</span><span class="sxs-lookup"><span data-stu-id="fcc5d-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="fcc5d-103">Σύνδεση AD Azure (έκδοση 1.1.524.0 και μετά) τώρα διευκολύνει τη χρήση των ΜΣΠ-συνεπή Encyguid ως χαρακτηριστικό sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="fcc5d-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="fcc5d-104">Όταν χρησιμοποιείτε αυτήν τη δυνατότητα, σύνδεση AD Azure ρυθμίζει αυτόματα τους κανόνες συγχρονισμού για να:</span><span class="sxs-lookup"><span data-stu-id="fcc5d-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="fcc5d-105">Χρησιμοποιήστε τη χρήση ΜΣΠ-Ενκύμ_guid ως το χαρακτηριστικό Sourceαγκυρα για αντικείμενα χρήστη.</span><span class="sxs-lookup"><span data-stu-id="fcc5d-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="fcc5d-106">Η Object GUID χρησιμοποιείται για άλλους τύπους αντικειμένων.</span><span class="sxs-lookup"><span data-stu-id="fcc5d-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="fcc5d-107">Για οποιαδήποτε δεδομένη εσωτερικής εγκατάστασης αντικείμενο AD χρήστη του οποίου το χαρακτηριστικό ΜΣΠ-συνέπειας Encyguid δεν συμπληρώνεται, σύνδεση AD Azure εγγράφει την τιμή αντικειμένου αντικειμένων του πίσω στο χαρακτηριστικό ΜΣΠ-συνεπή Encyguid σε εσωτερικής εγκατάστασης Active Directory.</span><span class="sxs-lookup"><span data-stu-id="fcc5d-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="fcc5d-108">Αφού συμπληρωθεί το χαρακτηριστικό ΜΣΠ-συνέπειας GUID, σύνδεση AD Azure, στη συνέχεια, εξάγει το αντικείμενο σε Azure AD.</span><span class="sxs-lookup"><span data-stu-id="fcc5d-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="fcc5d-109">**Σημείωση:** Όταν ένα αντικείμενο AD εσωτερικής εγκατάστασης εισάγεται σε σύνδεση AD Azure (δηλαδή, εισάγεται στο χώρο σύνδεσης AD και προπροβάλλεται σε το Mevce), δεν μπορείτε να αλλάξετε την τιμή του sourceAnchor πλέον.</span><span class="sxs-lookup"><span data-stu-id="fcc5d-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="fcc5d-110">Για να καθορίσετε την τιμή Υποαγκύρωσης για ένα δεδομένο αντικείμενο AD εσωτερικής εγκατάστασης, ρυθμίστε το χαρακτηριστικό του ΜΣΠ-συνέπειας Encyto GUID πριν να εισαχθεί σε σύνδεση AD Azure.</span><span class="sxs-lookup"><span data-stu-id="fcc5d-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="fcc5d-111">Για περισσότερες πληροφορίες σχετικά με την Αγκυρα αγκύρωσης και τη συνεπή Encyguid, ανατρέξτε στα ακόλουθα: [Azure AD Connect: έννοιες σχεδίασης](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="fcc5d-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

