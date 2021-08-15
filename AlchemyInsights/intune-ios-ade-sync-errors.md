---
title: Σφάλματα συγχρονισμού αυτόματης εγγραφής συσκευών apple
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
- "9000654"
- "7256"
ms.openlocfilehash: 1664a26b313c4a38c9c6d78cdb89997749ba175fd3dd72f278e99bbd50b0ee84
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013748"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Σφάλματα συγχρονισμού αυτόματης εγγραφής συσκευών apple

"Εντοπίσαμε ότι έχετε ένα ή περισσότερα διακριτικά ADE/DEP που βρίσκονται σε κατάσταση σφάλματος. Μέχρι να επιλυθεί η κατάσταση σφάλματος για κάθε διακριτικό που επηρεάζεται, η λειτουργικότητα ADE δεν θα λειτουργεί όπως αναμένεται.".

Αυτό το σφάλμα μπορεί να εμφανιστεί με διάφορους τρόπους, όπως:

1. Οι συσκευές ενδέχεται να μην συγχρονίζονται από ABM/ASM σε Intune
2. Οι αναθέσεις εργασιών προφίλ εγγραφής ενδέχεται να αποτυγχάνουν
3. Οι συσκευές ενδέχεται να μην ολοκληρώσουν την εγγραφή ADE με επιτυχία

Ελέγξτε για το σφάλμα συγχρονισμού που αναφέρεται στην κονσόλα Intune στην περιοχή Συσκευές **> Εγγραφή συσκευών > Διακριτικά προγράμματος >** εγγραφής Apple.

Μία από τις πιο συνηθισμένες αιτίες σφάλματος συγχρονισμού είναι η λήξη του τρέχοντος διακριτικού. Σε πολλές περιπτώσεις, η ανανέωση του διακριτικού που επηρεάζεται θα επιλύσει το πρόβλημα.

Εάν ένα ή περισσότερα από τα διακριτικά σας έχουν λήξει, ανατρέξτε στην παρακάτω τεκμηρίωση για να σας βοηθήσουν να τα ανανεώσετε ανάλογα με την περίπτωση:

[Ανανέωση διακριτικού αυτόματης εγγραφής συσκευής](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

Επιπλέον, μπορείτε να δείτε την παρακάτω τεκμηρίωση για να δείτε πιθανές αποκατάστασης εύρυθμης λειτουργίας για άλλα σφάλματα που προκαλούν αποτυχίες συγχρονισμού διακριτικών:

[Σφάλματα συγχρονισμού ABM/ASM για διακριτικά αυτόματης εγγραφής συσκευών iOS/iPadOS και macOS](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[Σφάλματα συγχρονισμού ABM/ASM για διακριτικά αυτόματης εγγραφής συσκευών iOS/iPadOS και macOS](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
