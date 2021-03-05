---
title: Πρόβλημα με το AAD Connect Health
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
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481467"
---
# <a name="problem-with-aad-connect-health"></a>Πρόβλημα με το AAD Connect Health

- Βεβαιωθείτε ότι είστε εξουσιοδοτημένοι για την εκτέλεση της λειτουργίας. Οι καθολικοί διαχειριστές έχουν πρόσβαση από προεπιλογή. Επιπλέον, μπορείτε να χρησιμοποιήσετε τον Έλεγχο πρόσβασης βάσει [ρόλων για να](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) αναθέσετε δικαιώματα καταχώρησης στον Συνεργάτη.
- Βεβαιωθείτε ότι τα απαιτούμενα τελικά σημεία είναι ενεργοποιημένα και δεν έχουν αποκλειστεί λόγω του τείχους προστασίας. Για λεπτομέρειες, ανατρέξτε στις [απαιτήσεις.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)
- Η καταχώρηση μπορεί να αποτύχει λόγω του ότι η εξερχόμενη επικοινωνία υπόκειται σε έλεγχο SSL από το επίπεδο δικτύου.
- Βεβαιωθείτε ότι έχετε επαληθεύσει τις ρυθμίσεις ειδοποιήσεων για το Azure AD Connect Health. Ελέγξτε τη ρυθμίσεών σας. Αυτός ο [οδηγός μπορεί](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) να σας βοηθήσει να κατανοήσετε πώς μπορείτε να ρυθμίσετε τις παραμέτρους ειδοποιήσεων για ειδοποιήσεις σχετικά με την κατάσταση του Azure AD Connect.
- Για να μάθετε περισσότερα σχετικά με την αναφορά συγχρονισμού της υγείας του AAD Connect και τον τρόπο λήψης της, ανατρέξτε στην [αναφορά συγχρονισμού επιπέδου αντικειμένου.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)

Για την αντιμετώπιση προβλημάτων με τις ειδοποιήσεις υγείας του AAD Connect, ακολουθήστε τον οδηγό αντιμετώπισης προβλημάτων για τις ειδοποιήσεις πιο πρόσφατα δεδομένα του [AAD Connect Health](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) και για συνήθεις ερωτήσεις, ανατρέξτε στις συνήθεις ερωτήσεις σχετικά με την εγκατάσταση του [AAD Connect Health.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)
