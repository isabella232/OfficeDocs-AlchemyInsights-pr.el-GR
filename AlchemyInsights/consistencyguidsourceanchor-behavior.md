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
# <a name="consistencyguid--sourceanchor-behavior"></a>Συμπεριφορά ConsistencyGuid /sourceAnchor

Το Azure AD Connect (έκδοση 1.1.524.0 και μετά) διευκολύνει πλέον τη χρήση του msDS-ConsistencyGuid ως χαρακτηριστικού sourceAnchor. Κατά τη χρήση αυτής της δυνατότητας, το Azure AD Connect ρυθμίζει αυτόματα τις παραμέτρους των κανόνων συγχρονισμού ώστε:
  
- Χρησιμοποιήστε το msDS-ConsistencyGuid ως το χαρακτηριστικό sourceAnchor για αντικείμενα χρήστη. Το ObjectGUID χρησιμοποιείται για άλλους τύπους αντικειμένων.
    
- Για οποιοδήποτε δεδομένο αντικείμενο χρήστη AD εσωτερικής εγκατάστασης του οποίου το χαρακτηριστικό msDS-ConsistencyGuid δεν έχει συμπληρωθεί, το Azure AD Connect επιστρέφει την τιμή objectGUID στο χαρακτηριστικό msDS-ConsistencyGuid στην υπηρεσία καταλόγου Active Directory εσωτερικής εγκατάστασης. Μετά τη συμπλήρωση του χαρακτηριστικού msDS-ConsistencyGuid, το Azure AD Connect εξάγει το αντικείμενο στο Azure AD.
    
 **Σημείωση:** Μετά την εισαγωγή ενός αντικειμένου AD εσωτερικής εγκατάστασης στο Azure AD Connect (δηλαδή, εισάγεται στο χώρο σύνδεσης AD και προ βλάφεται στο Μετα-στίχο), δεν μπορείτε πλέον να αλλάξετε την τιμή sourceAnchor. Για να καθορίσετε την τιμή sourceAnchor για ένα δεδομένο αντικείμενο AD εσωτερικής εγκατάστασης, ρυθμίστε τις παραμέτρους του χαρακτηριστικού msDS-ConsistencyGuid πριν από την εισαγωγή του στο Azure AD Connect. 
  
Για περισσότερες πληροφορίες σχετικά με το SourceAnchor και το ConsistencyGuid, ανατρέξτε στα εξής: [Azure AD Connect: Έννοιες σχεδίασης](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

