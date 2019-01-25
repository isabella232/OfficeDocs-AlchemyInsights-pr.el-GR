---
title: ConsistencyGuid / sourceAnchor συμπεριφορά
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: 80516ed9e15040475a8b65a1af98a1b561704d49
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29498518"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / sourceAnchor συμπεριφορά

Σύνδεση AD Azure (έκδοση 1.1.524.0 και μετά) τώρα διευκολύνει τη χρήση msDS-ConsistencyGuid ως χαρακτηριστικό sourceAnchor. Όταν χρησιμοποιείτε αυτήν τη δυνατότητα, σύνδεση AD Azure ρυθμίζει αυτόματα τις παραμέτρους των κανόνων συγχρονισμού για να:
  
- Χρησιμοποιήστε msDS-ConsistencyGuid με το χαρακτηριστικό sourceAnchor για αντικείμενα χρήστη. ObjectGUID χρησιμοποιείται για άλλους τύπους αντικειμένου.
    
- Για οποιαδήποτε λόγω εσωτερικής εγκατάστασης χρήστη AD αντικείμενο του οποίου το χαρακτηριστικό msDS-ConsistencyGuid δεν είναι συμπληρωμένη, Azure AD σύνδεση εγγράφει την τιμή objectGUID πίσω στο χαρακτηριστικό msDS-ConsistencyGuid εσωτερικής εγκατάστασης υπηρεσίας καταλόγου Active Directory. Αφού συμπληρωθεί το χαρακτηριστικό msDS-ConsistencyGuid, σύνδεση AD Azure εξάγει, στη συνέχεια, το αντικείμενο Azure AD.
    
 **Σημείωση:** Μία φορά μια ενδοεταιρική αντικείμενο AD εισάγεται στη σύνδεση AD Azure (δηλαδή, εισάγονται στο χώρο της σύνδεσης AD και πρόβλεψη σε το Metaverse), δεν μπορείτε να αλλάξετε την τιμή της sourceAnchor πλέον. Για να καθορίσετε την τιμή sourceAnchor για μια λόγω εσωτερικής εγκατάστασης AD αντικειμένων, να ρυθμίσετε τις παραμέτρους του χαρακτηριστικού msDS-ConsistencyGuid, πριν από την εισαγωγή σε σύνδεση AD Azure. 
  
Για περισσότερες πληροφορίες σχετικά με SourceAnchor και ConsistencyGuid, ανατρέξτε στα παρακάτω: [σύνδεση AD Azure: Σχεδίαση έννοιες](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

