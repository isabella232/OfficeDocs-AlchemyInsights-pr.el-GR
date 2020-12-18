---
title: Σφάλματα συγχρονισμού εγγραφής αυτόματης συσκευής Apple
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: d7a9398046a1073e30fdbe2950f750bb55d4fa2f
ms.sourcegitcommit: 87c8d0a1e6668211b9dd5427f98984ccdcadb02d
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 12/17/2020
ms.locfileid: "49714835"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Σφάλματα συγχρονισμού εγγραφής αυτόματης συσκευής Apple

"Εντοπίσαμε ότι έχετε ένα ή περισσότερα διακριτικά ADE/DEP που βρίσκονται σε κατάσταση σφάλματος. Μέχρι να επιλυθεί η κατάσταση σφάλματος για κάθε διακριτικό που επηρεάζεται, η λειτουργικότητα ADE δεν θα λειτουργεί για το ίδιο ".

Αυτό το σφάλμα μπορεί να εκδηλωθεί με διάφορους τρόπους, όπως:

1. Οι συσκευές ενδέχεται να μην συγχρονίζονται από το ΔΒΔ/από το Intune στο Intune
2. Οι αναθέσεις προφίλ εγγραφής ενδέχεται να μην είναι δυνατό να αποτύχουν
3. Οι συσκευές ενδέχεται να μην ολοκληρώσουν επιτυχώς την εγγραφή ADE

Ελέγξτε για το σφάλμα συγχρονισμού που αναφέρεται στην κονσόλα Intune στην περιοχή **συσκευές > εγγραφή συσκευών > εγγραφή Apple > κουπόνια προγράμματος εγγραφής** και εξετάστε την παρακάτω τεκμηρίωση για να δείτε τυχόν ενδεχόμενη επιδιόρθωση:

[Σφάλματα συγχρονισμού ΔΒΔ/τα για iOS/iPadOS και macOS αυτοματοποιημένων διακριτικών εγγραφής συσκευής](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
