---
title: Παρουσιάστηκε σφάλμα κατά την επικύρωση του σφάλματος διακριτικού πρόσβασης κατά τη διάρκεια της επιβίβασης στην ανάλυση υπολογιστή
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 45c6fb1a1632799a07c028c0791b6b8e77635293
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783551"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Σφάλμα "Παρουσιάστηκε σφάλμα κατά την επικύρωση του διακριτικού πρόσβασης" κατά τη διάρκεια της επιβίβασης στην ανάλυση επιφάνειας εργασίας

Αυτό το σφάλμα παρατηρείται συνήθως κατά τη λήξη του διακριτικού ελέγχου ταυτότητας. Συνήθως, η ανανέωση της σελίδας ανανεώνει το διακριτικό. Ωστόσο, αυτό το πρόβλημα μπορεί να συνεχιστεί εάν υπάρχουν πολιτικές πρόσβασης υπό όρους που εφαρμόζονται στο λογαριασμό που χρησιμοποιείται για την ενσωματωμένη ανάλυση υπολογιστή του υπολογιστή. Μπορείτε να εξετάσετε τα αρχεία καταγραφής του Azure AD Sign in στην πύλη Azure για να δείτε εάν υπάρχουν τυχόν αποτυχίες εισόδου για το λογαριασμό που χρησιμοποιείται για την επιβίβαση στην ανάλυση επιφάνειας εργασίας.

Για περισσότερες πληροφορίες σχετικά με την πρόσβαση υπό όρους, ανατρέξτε στο θέμα [Προγραμματισμός της ανάπτυξης της Access υπό όρους](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).