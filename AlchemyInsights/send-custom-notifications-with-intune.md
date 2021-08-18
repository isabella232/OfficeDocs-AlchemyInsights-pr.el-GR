---
title: Αποστολή προσαρμοσμένων ειδοποιήσεων με το Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 58acaa29f9d0b066cc7be6f6ee57b1806d0e8812b194e20166b133b7715226a8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54086164"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Τρόπος αποστολής προσαρμοσμένων ειδοποιήσεων στους χρήστες διαχειριζόμενων συσκευών iOS και Android

Οι προσαρμοσμένες ειδοποιήσεις για το Intune υποβάλλονται σε επεξεργασία από Εταιρική πύλη εφαρμογή στη συσκευή ενός χρήστη. Στη συνέχεια, η εφαρμογή δημιουργεί την ειδοποίηση push σε αυτήν τη συσκευή.

Ακολουθούν τα προαπαιτούμενα της συσκευής για την υποστήριξη της παραλαβής προσαρμοσμένων ειδοποιήσεων και, στη συνέχεια, η εφαρμογή να δημιουργήσει την ειδοποίηση push:

- Η συσκευή πρέπει να έχει εγκατεστημένη Εταιρική πύλη εφαρμογή.  

- Η συσκευή πρέπει να επιτρέπει στην Εταιρική πύλη να στέλνει ειδοποιήσεις push. Όταν η εφαρμογή εγκατασταθεί ή ενημερωθεί, θα ζητήσει από το χρήστη να επιτρέψει ειδοποιήσεις.

- Οι συσκευές Android πρέπει να έχουν εγκατεστημένες τις Υπηρεσίες Google Play.

- Η συσκευή πρέπει να είναι εγγεγραμμένη με το Intune.

Για περισσότερες πληροφορίες, συμπεριλαμβανομένου του πώς μπορείτε να στείλετε ένα μήνυμα, ανατρέξτε στην [τεκμηρίωση δυνατοτήτων.](https://docs.microsoft.com/intune/custom-notifications)
