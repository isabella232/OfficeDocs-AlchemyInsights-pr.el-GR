---
title: ΣυνέπειαGuid / συμπεριφορά sourceAnchor
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: 8527e7c2404742a999041f85ed12d78c48cc0d8c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43705733"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ΣυνέπειαGuid / συμπεριφορά sourceAnchor

Το Azure AD Connect (έκδοση 1.1.524.0 και μετά) διευκολύνει τώρα τη χρήση του msDS-ConsistencyGuid ως χαρακτηριστικού sourceAnchor. Όταν χρησιμοποιείτε αυτήν τη δυνατότητα, το Azure AD Connect ρυθμίζει αυτόματα τις παραμέτρους των κανόνων συγχρονισμού με:
  
- Χρησιμοποιήστε το msDS-ConsistencyGuid ως χαρακτηριστικό sourceAnchor για αντικείμενα χρήστη. Το ObjectGUID χρησιμοποιείται για άλλους τύπους αντικειμένων.
    
- Για οποιοδήποτε δεδομένο αντικείμενο χρήστη AD εσωτερικής εγκατάστασης του οποίου το χαρακτηριστικό msDS-ConsistencyGuid δεν έχει συμπληρωθεί, το Azure AD Connect εγγράφει την τιμή objectGUID στο χαρακτηριστικό msDS-ConsistencyGuid στην υπηρεσία καταλόγου Active Directory εσωτερικής εγκατάστασης. Μετά τη συμπλήρωση του χαρακτηριστικού msDS-ConsistencyGuid, το Azure AD Connect εξάγει το αντικείμενο σε Azure AD.
    
 **Σημείωση:** Μόλις εισαχθεί ένα αντικείμενο AD εσωτερικής εγκατάστασης στο Azure AD Connect (δηλαδή, εισάγεται στο χώρο σύνδεσης ad και προβάλλεται στο Metaverse), δεν μπορείτε πλέον να αλλάξετε την τιμή sourceAnchor. Για να καθορίσετε την τιμή sourceAnchor για ένα δεδομένο αντικείμενο AD εσωτερικής εγκατάστασης, ρυθμίστε τις παραμέτρους του χαρακτηριστικού msDs-ConsistencyGuid πριν από την εισαγωγή του στη Σύνδεση Azure AD. 
  
Για περισσότερες πληροφορίες σχετικά με το SourceAnchor και το ConsistencyGuid, ανατρέξτε στα εξής: [Azure AD Connect: Έννοιες σχεδίασης](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

