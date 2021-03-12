---
title: Αντιμετώπιση προβλημάτων εγκατάστασης MDATP σε Mac
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746304"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>Αντιμετώπιση προβλημάτων εγκατάστασης MDATP σε Mac

Εάν αποτύχει η μη αυτόματη εγκατάσταση, **η σελίδα** "Σύνοψη" του οδηγού εγκατάστασης εμφανίζει το ακόλουθο σφάλμα:

"Παρουσιάστηκε σφάλμα κατά την εγκατάσταση. Το πρόγραμμα εγκατάστασης αντιμετώπισε ένα σφάλμα που προκάλεσε την αποτυχία της εγκατάστασης. Επικοινωνήστε με τον κατασκευαστή του λογισμικού για βοήθεια."

Για αναπτύξεις MDM, η σελίδα εμφανίζει επίσης μια γενική αποτυχία εγκατάστασης.

Παρόλο που δεν εμφανίζονται ακριβή σφάλματα στους τελικούς χρήστες, διατηρείμε ένα αρχείο καταγραφής με την πρόοδο της εγκατάστασης, στο **/Library/Logs/Microsoft/mdatp/install.log.** Κάθε περίοδος λειτουργίας εγκατάστασης προσαρτάται σε αυτό το αρχείο καταγραφής. Για να κάνετε έξοδο μόνο στην τελευταία περίοδο λειτουργίας εγκατάστασης, χρησιμοποιήστε `sed` το .

Για να μάθετε περισσότερα, ανατρέξτε στο θέμα Αντιμετώπιση προβλημάτων εγκατάστασης για [το Microsoft Defender ATP για Mac.](https://go.microsoft.com/fwlink/?linkid=2144615)
