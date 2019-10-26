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
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 10/25/2019
ms.locfileid: "36516981"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>Συμπεριφορά αγκύρωσης/προέλευσης

Σύνδεση AD Azure (έκδοση 1.1.524.0 και μετά) τώρα διευκολύνει τη χρήση των ΜΣΠ-συνεπή Encyguid ως χαρακτηριστικό sourceAnchor. Όταν χρησιμοποιείτε αυτήν τη δυνατότητα, σύνδεση AD Azure ρυθμίζει αυτόματα τους κανόνες συγχρονισμού για να:
  
- Χρησιμοποιήστε τη χρήση ΜΣΠ-Ενκύμ_guid ως το χαρακτηριστικό Sourceαγκυρα για αντικείμενα χρήστη. Η Object GUID χρησιμοποιείται για άλλους τύπους αντικειμένων.
    
- Για οποιαδήποτε δεδομένη εσωτερικής εγκατάστασης αντικείμενο AD χρήστη του οποίου το χαρακτηριστικό ΜΣΠ-συνέπειας Encyguid δεν συμπληρώνεται, σύνδεση AD Azure εγγράφει την τιμή αντικειμένου αντικειμένων του πίσω στο χαρακτηριστικό ΜΣΠ-συνεπή Encyguid σε εσωτερικής εγκατάστασης Active Directory. Αφού συμπληρωθεί το χαρακτηριστικό ΜΣΠ-συνέπειας GUID, σύνδεση AD Azure, στη συνέχεια, εξάγει το αντικείμενο σε Azure AD.
    
 **Σημείωση:** Όταν ένα αντικείμενο AD εσωτερικής εγκατάστασης εισάγεται σε σύνδεση AD Azure (δηλαδή, εισάγεται στο χώρο σύνδεσης AD και προπροβάλλεται σε το Mevce), δεν μπορείτε να αλλάξετε την τιμή του sourceAnchor πλέον. Για να καθορίσετε την τιμή Υποαγκύρωσης για ένα δεδομένο αντικείμενο AD εσωτερικής εγκατάστασης, ρυθμίστε το χαρακτηριστικό του ΜΣΠ-συνέπειας Encyto GUID πριν να εισαχθεί σε σύνδεση AD Azure. 
  
Για περισσότερες πληροφορίες σχετικά με την Αγκυρα αγκύρωσης και τη συνεπή Encyguid, ανατρέξτε στα ακόλουθα: [Azure AD Connect: έννοιες σχεδίασης](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

