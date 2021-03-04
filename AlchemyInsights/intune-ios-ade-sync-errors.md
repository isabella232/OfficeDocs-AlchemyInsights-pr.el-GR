---
title: Σφάλματα συγχρονισμού αυτόματης εγγραφής συσκευών της Apple
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
ms.openlocfilehash: 912c9e56b4c468fb333769f15bd7c212594dc11a
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448922"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Σφάλματα συγχρονισμού αυτόματης εγγραφής συσκευών της Apple

"Εντοπίσαμε ότι έχετε ένα ή περισσότερα διακριτικά ADE/DEP που βρίσκονται σε κατάσταση σφάλματος. Μέχρι να επιλυθεί η κατάσταση σφάλματος για κάθε διακριτικό που επηρεάζεται, η λειτουργικότητα ADE δεν θα λειτουργεί όπως αναμένεται.".

Αυτό το σφάλμα ενδέχεται να εμφανιστεί με διάφορους τρόπους, όπως:

1. Οι συσκευές ενδέχεται να μην συγχρονίζονται από ABM/ASM στο Intune
2. Οι αναθέσεις προφίλ εγγραφής ενδέχεται να αποτυγχάνουν
3. Οι συσκευές ενδέχεται να μην ολοκληρώσουν την εγγραφή ADE με επιτυχία

Ελέγξτε για το σφάλμα συγχρονισμού που αναφέρθηκε στην κονσόλα Intune στην περιοχή Συσκευές **> Εγγραφή συσκευών > διακριτικά εγγραφής >** προγράμματος εγγραφής Apple.

Μία από τις πιο συνηθισμένες αιτίες του σφάλματος συγχρονισμού είναι η λήξη του τρέχοντος διακριτικού. Σε πολλές περιπτώσεις, η ανανέωση του διακριτικού που επηρεάζεται θα επιλύσει το πρόβλημα.

Εάν ένα ή περισσότερα από τα διακριτικά σας έχουν λήξει, ανατρέξτε στην ακόλουθη τεκμηρίωση που θα σας βοηθήσει να τα ανανεώσετε ανάλογα με την περίπτωση:

[Ανανέωση διακριτικού αυτόματης εγγραφής συσκευής](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

Επιπλέον, μπορείτε να δείτε την ακόλουθη τεκμηρίωση για να δείτε πιθανές αποκατάσταση για άλλα σφάλματα που προκαλούν αποτυχίες συγχρονισμού διακριτικών:

[Σφάλματα συγχρονισμού ABM/ASM για διακριτικά εγγραφής αυτοματοποιημένων συσκευών για iOS/iPadOS και macOS](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[Σφάλματα συγχρονισμού ABM/ASM για διακριτικά εγγραφής αυτοματοποιημένων συσκευών για iOS/iPadOS και macOS](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
