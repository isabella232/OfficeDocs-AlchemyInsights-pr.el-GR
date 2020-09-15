---
title: Σφάλμα AttributeValueMustBeUnique
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
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 4627a7ae34b0dd9f16538ef75ac8792672dcc056
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709151"
---
# <a name="error-attributevaluemustbeunique"></a>Σφάλμα: AttributeValueMustBeUnique

Ο πιο συνηθισμένος λόγος για το σφάλμα AttributeValueMustBeUnique είναι δύο αντικείμενα με διαφορετικές SourceAnchor (immutableId) έχουν την ίδια τιμή για τα χαρακτηριστικά του ProxyAddresses ή/και του UserPrincipalName. Για να διορθώσετε το σφάλμα AttributeValueMustBeUnique:
  
1. Προσδιορίστε την διπλότυπη proxyAddresses, userPrincipalName ή άλλη τιμή χαρακτηριστικού που προκαλεί το σφάλμα. Επίσης, Προσδιορίστε ποια δύο (ή περισσότερα) αντικείμενα εμπλέκονται στη διένεξη. Η αναφορά που δημιουργείται από την εύρυθμη λειτουργία του Azure AD Connect για συγχρονισμό μπορεί να σας βοηθήσει να προσδιορίσετε τα δύο αντικείμενα.
    
2. Προσδιορίστε ποιο αντικείμενο πρέπει να συνεχίσει να έχει την διπλότυπη τιμή και ποιο αντικείμενο δεν πρέπει να έχει.
    
3. Καταργήστε την διπλότυπη τιμή από το αντικείμενο που δεν θα πρέπει να έχει αυτήν την τιμή. Σημειώστε ότι θα πρέπει να κάνετε την αλλαγή στον κατάλογο από τον οποίο προέρχεται το αντικείμενο. Σε ορισμένες περιπτώσεις, ίσως χρειαστεί να διαγράψετε ένα από τα αντικείμενα που βρίσκονται σε διένεξη.
    
4. Εάν κάνατε την αλλαγή στη διαφήμιση του χώρου, αφήστε το Azure AD Connect να συγχρονίσει την αλλαγή για να διορθωθεί το σφάλμα.
    

