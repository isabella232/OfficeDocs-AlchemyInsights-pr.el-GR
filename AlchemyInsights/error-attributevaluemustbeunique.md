---
title: Σφάλμα AttributeValueMustBeUnique
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
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 35eb88624a5535e136ac1d01faf8e905bf00eb45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813760"
---
# <a name="error-attributevaluemustbeunique"></a>Σφάλμα: AttributeValueMustBeUnique

Ο πιο συνηθισμένος λόγος για το σφάλμα AttributeValueMustBeUnique είναι ότι δύο αντικείμενα με διαφορετικό SourceAnchor (immutableId) έχουν την ίδια τιμή για τα χαρακτηριστικά ProxyAddresses ή/και UserPrincipalName. Για να διορθώσετε το σφάλμα AttributeValueMustBeUnique:
  
1. Προσδιορίστε τις διπλότυπες proxyAddresses, userPrincipalName ή άλλη τιμή χαρακτηριστικού που προκαλεί το σφάλμα. Επίσης, προσδιορίστε ποια δύο (ή περισσότερα) αντικείμενα εμπλέκονται στη διένεξη. Η αναφορά που δημιουργείται από το Azure AD Connect Health για συγχρονισμό μπορεί να σας βοηθήσει να προσδιορίσετε τα δύο αντικείμενα.
    
2. Προσδιορίστε ποιο αντικείμενο θα πρέπει να συνεχίσει να έχει την διπλότυπη τιμή και ποιο αντικείμενο δεν θα πρέπει να έχει.
    
3. Καταργήστε την διπλότυπη τιμή από το αντικείμενο που ΔΕΝ θα πρέπει να έχει αυτή την τιμή. Σημειώστε ότι θα πρέπει να κάνετε την αλλαγή στον κατάλογο από τον οποίο προέρχεται το αντικείμενο. Σε ορισμένες περιπτώσεις, ίσως χρειαστεί να διαγράψετε ένα από τα αντικείμενα σε διένεξη.
    
4. Εάν κάνατε την αλλαγή στο AD εσωτερικής εγκατάστασης, αφήστε το Azure AD Connect να συγχρονίσει την αλλαγή για να διορθωθεί το σφάλμα.
    

