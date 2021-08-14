---
title: Πρόβλημα με το AAD Σύνδεση Υγείας
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004649"
- "8427"
ms.openlocfilehash: 82cfcc6132549b52278b174fce3173f5566268864a207882a4dd639cb8024ee3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923752"
---
# <a name="problem-with-aad-connect-health"></a>Πρόβλημα με το AAD Σύνδεση Υγείας

- Βεβαιωθείτε ότι έχετε εξουσιοδότηση για την εκτέλεση της λειτουργίας. Οι καθολικοί διαχειριστές έχουν πρόσβαση από προεπιλογή. Επιπλέον, μπορείτε να χρησιμοποιήσετε τον Έλεγχο πρόσβασης βάσει [ρόλων για να](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) αναθέσετε δικαιώματα καταχώρησης στον Συνεργάτη.
- Βεβαιωθείτε ότι τα απαιτούμενα τελικά σημεία είναι ενεργοποιημένα και δεν αποκλείονται λόγω του τείχους προστασίας. Για λεπτομέρειες, ανατρέξτε στις [απαιτήσεις.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)
- Η εγγραφή μπορεί να αποτύχει, επειδή η εξερχόμενη επικοινωνία υπόκειται σε έλεγχο SSL από το επίπεδο δικτύου.
- Βεβαιωθείτε ότι έχετε επαληθεύσει τις ρυθμίσεις ειδοποιήσεων για το Azure AD Σύνδεση Υγείας. Ελέγξτε τη ρυθμίσετε. Αυτός [ο οδηγός](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) μπορεί να σας βοηθήσει να κατανοήσετε πώς μπορείτε να ρυθμίσετε τις παραμέτρους ειδοποιήσεων για το Azure AD Σύνδεση ειδοποιήσεις υγείας.
- Για να μάθετε περισσότερα σχετικά με την αναφορά συγχρονισμού Σύνδεση AAD και τον τρόπο λήψης της, ανατρέξτε στην αναφορά συγχρονισμού [επιπέδου αντικειμένου.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)

Για να αντιμετωπίσετε προβλήματα με τις ειδοποιήσεις AAD Σύνδεση Health, ακολουθήστε τον οδηγό αντιμετώπισης προβλημάτων για τις ειδοποιήσεις φρεσκάδας δεδομένων υγείας [του AAD Σύνδεση](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) και για συνήθεις ερωτήσεις, ανατρέξτε στο θέμα Συνήθεις ερωτήσεις σχετικά με [την εγκατάσταση του AAD Σύνδεση υγείας.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)
