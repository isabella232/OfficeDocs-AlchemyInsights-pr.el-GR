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
ms.openlocfilehash: 2e5e2e2f24c46d3db4f08862dcc80934937f6f51
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720646"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Πώς μπορείτε να στείλετε προσαρμοσμένες ειδοποιήσεις στους χρήστες διαχειριζόμενων συσκευών iOS και Android

Οι προσαρμοσμένες ειδοποιήσεις για το Intune υποβάλλονται σε επεξεργασία από την εφαρμογή εταιρεία πύλης στη συσκευή ενός χρήστη. Στη συνέχεια, η εφαρμογή δημιουργεί την ειδοποίηση push σε αυτήν τη συσκευή.

Ακολουθούν οι προϋποθέσεις συσκευής για την υποστήριξη της παραλαβής προσαρμοσμένων ειδοποιήσεων και, στη συνέχεια, η εφαρμογή θα δημιουργήσει την ειδοποίηση push:

- Η συσκευή πρέπει να έχει εγκατεστημένη την εφαρμογή εταιρεία πύλης.  

- Η συσκευή πρέπει να επιτρέπει στην εφαρμογή πύλης εταιρείας να στέλνει ειδοποιήσεις push. Κατά την εγκατάσταση ή την ενημέρωση της εφαρμογής, θα ζητηθεί από το χρήστη να επιτρέψει τις ειδοποιήσεις.

- Οι συσκευές Android πρέπει να έχουν εγκατεστημένο το Google Play Services.

- Η συσκευή πρέπει να είναι εγγεγραμμένη με το Intune.

Για περισσότερες πληροφορίες, όπως πώς μπορείτε να στείλετε ένα μήνυμα, ανατρέξτε στην [τεκμηρίωση της δυνατότητας](https://docs.microsoft.com/intune/custom-notifications).
