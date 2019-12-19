---
title: Παρουσιάστηκε σφάλμα κατά την επικύρωση του σφάλματος διακριτικού πρόσβασης κατά την επιβίβαση στην ανάλυση επιφάνειας εργασίας
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 7472af5c4e19e5697b5fb4802ed1cbb2c74f1d19
ms.sourcegitcommit: f1fad2129d09660ec42dbce03ce2c6b4cfc9555a
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 12/18/2019
ms.locfileid: "40741184"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Εμφανίζεται το μήνυμα λάθους "Παρουσιάστηκε σφάλμα επικύρωσης διακριτικού πρόσβασης" κατά τη διάρκεια της ανάλυσης επιφάνειας εργασίας

Αυτό το σφάλμα παρατηρείται συνήθως όταν λήξει το διακριτικό ελέγχου ταυτότητας. Συνήθως, η ανανέωση της σελίδας ανανεώνει το διακριτικό. Ωστόσο, αυτό το ζήτημα μπορεί να επιμείνει εάν υπάρχουν πολιτικές υπό όρους πρόσβασης που εφαρμόζονται στο λογαριασμό που χρησιμοποιείται για την ανάλυση επιφάνειας εργασίας επί του σκάφους. Μπορείτε να αναθεωρήσετε τα αρχεία καταγραφής σύνδεσης Azure AD στην πύλη Azure για να δείτε αν υπάρχουν τυχόν αποτυχίες εισόδου για το λογαριασμό που χρησιμοποιείται για την καταγραφή της ανάλυσης επιφάνειας εργασίας.

Για περισσότερες πληροφορίες σχετικά με την υπό όρους πρόσβαση, επισκεφθείτε [το πρόγραμμα ανάπτυξης υπό όρους πρόσβασης](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).