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
ms.openlocfilehash: 9b5765ff3c59b1312bead41a45a53478a96260df0567f006ab93c3ccfaf4be64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044340"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>Συμπεριφορά ConsistencyGuid /sourceAnchor

Το Azure AD Σύνδεση (έκδοση 1.1.524.0 και μετά) διευκολύνει πλέον τη χρήση του msDS-ConsistencyGuid ως χαρακτηριστικού sourceAnchor. Κατά τη χρήση αυτής της δυνατότητας, το Azure AD Σύνδεση ρυθμίζει αυτόματα τους κανόνες συγχρονισμού ώστε:
  
- Χρησιμοποιήστε το msDS-ConsistencyGuid ως το χαρακτηριστικό sourceAnchor για αντικείμενα χρήστη. Το ObjectGUID χρησιμοποιείται για άλλους τύπους αντικειμένων.
    
- Για οποιοδήποτε δεδομένο αντικείμενο χρήστη AD εσωτερικής εγκατάστασης του οποίου το χαρακτηριστικό msDS-ConsistencyGuid δεν έχει συμπληρωθεί, το Azure AD Σύνδεση επιστρέφει την τιμή objectGUID στο χαρακτηριστικό msDS-ConsistencyGuid στην υπηρεσία καταλόγου Active Directory εσωτερικής εγκατάστασης. Μετά τη συμπλήρωση του χαρακτηριστικού msDS-ConsistencyGuid, το Azure AD Σύνδεση, στη συνέχεια, εξάγει το αντικείμενο στο Azure AD.
    
 **Σημείωση:** Όταν ένα αντικείμενο AD εσωτερικής εγκατάστασης εισαχθεί στο Azure AD Σύνδεση (δηλαδή, εισάγεται στο χώρο της γραμμής σύνδεσης AD και είναι προβλεπόμενο στο Μετα-στίχο), δεν μπορείτε πλέον να αλλάξετε την τιμή προέλευσηςAnchor. Για να καθορίσετε την τιμή sourceAnchor για ένα δεδομένο αντικείμενο AD εσωτερικής εγκατάστασης, ρυθμίστε τις παραμέτρους του χαρακτηριστικού msDS-ConsistencyGuid πριν από την εισαγωγή του στο Azure AD Σύνδεση. 
  
Για περισσότερες πληροφορίες σχετικά με το SourceAnchor και το ConsistencyGuid, ανατρέξτε στα εξής: [Azure AD Σύνδεση: Έννοιες σχεδίασης](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

