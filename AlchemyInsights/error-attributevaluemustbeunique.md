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
ms.openlocfilehash: 37d6764d19d9cfbb0899a5ab85a4b1530896568adc364122075b7d6f2a32970a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54002120"
---
# <a name="error-attributevaluemustbeunique"></a>Σφάλμα: AttributeValueMustBeUnique

Ο πιο συνηθισμένος λόγος για το σφάλμα AttributeValueMustBeUnique είναι ότι δύο αντικείμενα με διαφορετικό SourceAnchor (immutableId) έχουν την ίδια τιμή για τα χαρακτηριστικά ProxyAddresses ή/και UserPrincipalName. Για να διορθώσετε το σφάλμα AttributeValueMustBeUnique:
  
1. Προσδιορίστε τις διπλότυπες proxyAddresses, userPrincipalName ή άλλη τιμή χαρακτηριστικού που προκαλεί το σφάλμα. Επίσης, προσδιορίστε ποια δύο (ή περισσότερα) αντικείμενα εμπλέκονται στη διένεξη. Η αναφορά που δημιουργείται από το Azure AD Σύνδεση για συγχρονισμό μπορεί να σας βοηθήσει να προσδιορίσετε τα δύο αντικείμενα.
    
2. Προσδιορίστε ποιο αντικείμενο θα πρέπει να συνεχίσει να έχει την διπλότυπη τιμή και ποιο αντικείμενο δεν θα πρέπει να έχει.
    
3. Καταργήστε την διπλότυπη τιμή από το αντικείμενο που ΔΕΝ θα πρέπει να έχει αυτή την τιμή. Σημειώστε ότι θα πρέπει να κάνετε την αλλαγή στον κατάλογο από τον οποίο προέρχεται το αντικείμενο. Σε ορισμένες περιπτώσεις, ίσως χρειαστεί να διαγράψετε ένα από τα αντικείμενα σε διένεξη.
    
4. Εάν κάνατε την αλλαγή στο AD εσωτερικής εγκατάστασης, αφήστε το Azure AD να Σύνδεση την αλλαγή για να διορθωθεί το σφάλμα.
    

