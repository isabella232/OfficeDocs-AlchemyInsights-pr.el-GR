---
title: Ειδοποίηση AAD Connect
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
- "9003245"
- "9326"
ms.openlocfilehash: 832c9dd587cb023b5b1d87e905acb123df34237f
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036112"
---
# <a name="notification-aad-connect"></a>Ειδοποίηση AAD Connect

- Βεβαιωθείτε ότι έχετε εξουσιοδότηση για την εκτέλεση της λειτουργίας. Οι καθολικοί διαχειριστές έχουν πρόσβαση από προεπιλογή. Επιπλέον, μπορείτε να χρησιμοποιήσετε τον Έλεγχο πρόσβασης βάσει [ρόλων για να](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) αναθέσετε δικαιώματα καταχώρησης στον Συνεργάτη.
- Βεβαιωθείτε ότι τα απαιτούμενα τελικά σημεία είναι ενεργοποιημένα και δεν αποκλείονται λόγω του τείχους προστασίας. Για λεπτομέρειες, ανατρέξτε στις [απαιτήσεις.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)
- Η εγγραφή μπορεί να αποτύχει, επειδή η εξερχόμενη επικοινωνία υπόκειται σε έλεγχο SSL από το επίπεδο δικτύου.
- Βεβαιωθείτε ότι έχετε επαληθεύσει τις ρυθμίσεις ειδοποιήσεων για το Azure AD Connect Health και ελέγξτε τη ρύθμιση. Για να κατανοήσετε πώς μπορείτε να ρυθμίσετε τις παραμέτρους ειδοποιήσεων για τις ειδοποιήσεις υγείας του Azure AD Connect, ανατρέξτε σε αυτόν [τον οδηγό.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations)
- Για να μάθετε περισσότερα σχετικά με την αναφορά συγχρονισμού AAD Connect Health και τον τρόπο λήψης της, ανατρέξτε στην αναφορά [συγχρονισμού επιπέδου αντικειμένου.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)

Για να αντιμετωπίσετε προβλήματα με τις ειδοποιήσεις υγείας του [AAD Connect,](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) ακολουθήστε τον οδηγό αντιμετώπισης προβλημάτων για τις ειδοποιήσεις φρεσκάδας δεδομένων του AAD Connect Health και για συνήθεις ερωτήσεις, ανατρέξτε στο θέμα Συνήθεις ερωτήσεις εγκατάστασης του [AAD Connect Health.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)
