---
title: Παρουσιάστηκε σφάλμα κατά την επικύρωση του διακριτικού πρόσβασης κατά την επιβιβα μένη ανάλυση επιφάνειας εργασίας
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 12e5906ba8cbc76ba1fd99dde1cf76396c3a6942
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813688"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Σφάλμα "Παρουσιάστηκε σφάλμα κατά την επικύρωση διακριτικού πρόσβασης" κατά την επιχείριση της Ανάλυσης επιφάνειας εργασίας

Αυτό το σφάλμα συνήθως παρατηρείται όταν λήξει το διακριτικό ελέγχου ταυτότητας. Συνήθως, η ανανέωση της σελίδας ανανεώνει το διακριτικό. Ωστόσο, αυτό το πρόβλημα μπορεί να συνεχιστεί εάν υπάρχουν πολιτικές πρόσβασης υπό όρους που εφαρμόζονται στο λογαριασμό που χρησιμοποιείται για την ανάλυση επιφάνειας εργασίας επί του πίνακα. Μπορείτε να εξετάσετε τα αρχεία καταγραφής εισόδου του Azure AD στην Πύλη Azure για να δείτε εάν υπάρχουν αποτυχίες εισόδου για το λογαριασμό που χρησιμοποιείται για την εγγραφή στο Desktop Analytics.

Για περισσότερες πληροφορίες σχετικά με την πρόσβαση υπό όρους, επισκεφθείτε την [τοποθεσία "Σχεδιασμός ανάπτυξης πρόσβασης υπό όρους".](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)