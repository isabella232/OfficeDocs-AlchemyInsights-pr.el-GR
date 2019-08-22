---
title: Σφάλμα AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 5ac56fa78c66cf3b246bc0cc01f040e27310d629
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36526994"
---
# <a name="error-attributevaluemustbeunique"></a>Σφάλμα: AttributeValueMustBeUnique

Ο πιο συνηθισμένος λόγος για το σφάλμα AttributeValueMustBeUnique είναι δύο αντικείμενα με διαφορετικές SourceAnchor (immutableId) έχουν την ίδια τιμή για τα χαρακτηριστικά ProxyAddresses ή/και UserPrincipalName. Για να διορθώσετε το σφάλμα AttributeValueMustBeUnique:
  
1. Προσδιορίζει το διπλότυπο proxyAddresses, userPrincipalName ή άλλη τιμή χαρακτηριστικού που προκαλεί το σφάλμα. Επίσης, προσδιορίστε ποια αντικείμενα δύο (ή περισσότερες) που έχουν σχέση με τη διένεξη. Η αναφορά που δημιουργείται από την υγεία σύνδεση AD Azure για συγχρονισμό σάς βοηθούν να προσδιορίσετε τα δύο αντικείμενα.
    
2. Να προσδιορίσετε ποιο αντικείμενο θα πρέπει να εξακολουθήσει να έχει την τιμή που αντιγράφηκε και ποιο αντικείμενο δεν θα έπρεπε.
    
3. Καταργήστε την τιμή που αντιγράφηκε από το αντικείμενο που θα πρέπει να έχει την τιμή. Σημειώστε ότι θα πρέπει να κάνετε την αλλαγή στον κατάλογο όπου η προέλευση του αντικειμένου από. Σε ορισμένες περιπτώσεις, ίσως χρειαστεί να διαγράψετε ένα από τα αντικείμενα που βρίσκονται σε διένεξη.
    
4. Εάν κάνατε την αλλαγή σε σε χώρους AD, σας επιτρέπουν να συγχρονίσετε την αλλαγή για το σφάλμα ώστε να διορθωθεί το Azure AD σύνδεση.
    

