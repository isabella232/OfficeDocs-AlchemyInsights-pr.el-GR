---
title: Διαγραφή ορφανού χρήστη από διακομιστή εσωτερικής εγκατάστασης
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 7927c0684d2f5289f92506d7d05d5b1a3b43b658
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 07/20/2020
ms.locfileid: "45198186"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a>Διαγραφή ορφανού χρήστη από διακομιστή εσωτερικής εγκατάστασης

Για να καταργήσετε έναν ορφανό χρήστη, ακολουθήστε τα εξής βήματα:

1. Επιβάλλετε το συγχρονισμό καταλόγου ακολουθώντας τις οδηγίες στην επιλογή [Τι είναι η υβριδική ταυτότητα με την υπηρεσία καταλόγου Azure Active Directory;](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).

2. Για να επαληθεύσετε το συγχρονισμό καταλόγου, ανατρέξτε στο θέμα [Τι είναι η υβριδική ταυτότητα με την υπηρεσία καταλόγου Azure Active Directory;](https://technet.microsoft.com/library/jj151797.aspx).

3. Εάν οι συναρτήσεις συγχρονισμού είναι σωστές, αλλά η διαγραφή αντικειμένου της υπηρεσίας καταλόγου Active Directory δεν μεταδίδεται στο Azure AD, καταργήστε με μη αυτόματο τρόπο το ορφανό αντικείμενο, χρησιμοποιώντας ένα από τα ακόλουθα cmdlet της λειτουργικής μονάδας azure active directory για windows PowerShell:

    Κατάργηση-MsolΕπικοίνετε  
    Κατάργηση-MsolGroup  
    Κατάργηση χρήστη-msol

    Για παράδειγμα, για να καταργήσετε ορφανά john.smith@contoso.com αναγνωριστικού χρήστη, το οποίο δημιουργήθηκε αρχικά χρησιμοποιώντας συγχρονισμό καταλόγου, εκτελέστε το cmdlet:

    Κατάργηση-MsolUser –UserPrincipalName John.Smith@Contoso.com