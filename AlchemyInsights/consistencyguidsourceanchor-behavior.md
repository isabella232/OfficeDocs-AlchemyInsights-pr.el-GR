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
# <a name="consistencyguid--sourceanchor-behavior"></a>Συμπεριφορά ConsistencyGuid/sourceAnchor

Το Azure AD Connect (έκδοση 1.1.524.0 και After) διευκολύνει πλέον τη χρήση των ΜΣΠ-ConsistencyGuid ως χαρακτηριστικό sourceAnchor. Όταν χρησιμοποιείτε αυτήν τη δυνατότητα, το Azure AD Connect ρυθμίζει αυτόματα τους κανόνες συγχρονισμού σε:
  
- Χρησιμοποιήστε τις ΜΣΠ-ConsistencyGuid ως το χαρακτηριστικό sourceAnchor για αντικείμενα χρήστη. Το ObjectGUID χρησιμοποιείται για άλλους τύπους αντικειμένων.
    
- Για οποιοδήποτε συγκεκριμένο αντικείμενο AD εσωτερικής εγκατάστασης του οποίου το χαρακτηριστικό ΜΣΠ-ConsistencyGuid δεν είναι συμπληρωμένο, το Azure AD Connect καταγράφει την τιμή του objectGUID στο χαρακτηριστικό ΜΣΠ-ConsistencyGuid στην υπηρεσία καταλόγου Active Directory εσωτερικής εγκατάστασης. Μετά την συμπλήρωση του χαρακτηριστικού ΜΣΠ-ConsistencyGuid, το Azure AD Connect, στη συνέχεια, εξάγει το αντικείμενο στο Azure AD.
    
 **Σημείωση:** Μόλις εισαχθεί ένα αντικείμενο AD εσωτερικής εγκατάστασης στο Azure AD Connect (δηλαδή, έχει εισαχθεί στον χώρο σύνδεσης AD και προβληθεί στην Metaverse), δεν μπορείτε πλέον να αλλάξετε την τιμή του sourceAnchor. Για να καθορίσετε την τιμή sourceAnchor για ένα συγκεκριμένο αντικείμενο AD εσωτερικής εγκατάστασης, ρυθμίστε τις παραμέτρους του χαρακτηριστικού ΜΣΠ-ConsistencyGuid πριν από την εισαγωγή του στο Azure AD Connect. 
  
Για περισσότερες πληροφορίες σχετικά με το SourceAnchor και το ConsistencyGuid, ανατρέξτε στα εξής: [Azure AD Connect: έννοιες σχεδίασης](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

