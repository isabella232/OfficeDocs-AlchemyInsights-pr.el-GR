---
title: Το χαρακτηριστικό σφάλματοςValueMustBeUnique
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
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: fa1fdb35f1af250bc98aa61c0e5111f1f1b8aac4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703174"
---
# <a name="error-attributevaluemustbeunique"></a>Σφάλμα: ΧαρακτηριστικόΤιμήmustBeUnique

Ο πιο συνηθισμένος λόγος για το σφάλμα AttributeValueMustBeUnique είναι δύο αντικείμενα με διαφορετικό SourceAnchor (αμετάβλητοId) έχουν την ίδια τιμή για τις διευθύνσεις μεσολάβησης ή/και τα χαρακτηριστικά UserPrincipalName. Για να διορθώσετε το σφάλμα AttributeValueMustBeUnique:
  
1. Προσδιορίστε το διπλότυπο διακομιστή μεσολάβησηςΔιευθύνσεις, userPrincipalName ή άλλη τιμή χαρακτηριστικού που προκαλεί το σφάλμα. Επίσης, προσδιορίστε ποια δύο (ή περισσότερα) αντικείμενα εμπλέκονται στη διένεξη. Η αναφορά που δημιουργείται από την Εύρυθμη σύνδεση Azure AD για συγχρονισμό μπορεί να σας βοηθήσει να αναγνωρίσετε τα δύο αντικείμενα.
    
2. Προσδιορίστε ποιο αντικείμενο πρέπει να συνεχίσει να έχει την διπλότυπη τιμή και ποιο αντικείμενο δεν πρέπει.
    
3. Καταργήστε την διπλότυπη τιμή από το αντικείμενο που ΔΕΝ πρέπει να έχει αυτήν την τιμή. Σημειώστε ότι θα πρέπει να κάνετε την αλλαγή στον κατάλογο από τον οποίο προέρχεται το αντικείμενο. Σε ορισμένες περιπτώσεις, ίσως χρειαστεί να διαγράψετε ένα από τα αντικείμενα σε διένεξη.
    
4. Εάν κάνατε την αλλαγή στο AD εσωτερικής εγκατάστασης, αφήστε το Azure AD Connect να συγχρονίσει την αλλαγή για να διορθωθεί το σφάλμα.
    

