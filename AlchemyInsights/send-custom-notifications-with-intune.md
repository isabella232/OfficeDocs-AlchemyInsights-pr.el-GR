---
title: Αποστολή προσαρμοσμένων ειδοποιήσεων με το Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 969649084a2ac536ee1b41f225c3be5415a27c4b
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 12/27/2019
ms.locfileid: "40886857"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Πώς να στείλετε προσαρμοσμένες ειδοποιήσεις στους χρήστες των διαχειριζόμενων συσκευών iOS και Android

Οι προσαρμοσμένες ειδοποιήσεις για το Intune υποβάλλονται σε επεξεργασία από την εφαρμογή πύλης εταιρείας στη συσκευή ενός χρήστη. Στη συνέχεια, η εφαρμογή δημιουργεί την ειδοποίηση push σε αυτήν τη συσκευή.

Τα παρακάτω είναι προαπαιτούμενα συσκευών για την υποστήριξη παραλαβής προσαρμοσμένων ειδοποιήσεων και για την εφαρμογή στη συνέχεια να δημιουργήσετε την ειδοποίηση push:

- Η συσκευή πρέπει να έχει εγκατεστημένη την εφαρμογή πύλης εταιρείας.  

- Η συσκευή πρέπει να επιτρέπει στην εφαρμογή πύλης εταιρείας να αποστέλλει ειδοποιήσεις push. Όταν η εφαρμογή έχει εγκατασταθεί ή ενημερωθεί, θα ζητήσει από το χρήστη να επιτρέψει τις ειδοποιήσεις.

- Οι συσκευές Android πρέπει να έχουν εγκατεστημένες τις υπηρεσίες Google Play.

- Η συσκευή πρέπει να εγγραφεί στο Intune.

Για περισσότερες πληροφορίες, όπως πώς να στείλετε ένα μήνυμα, ανατρέξτε στην [τεκμηρίωση της δυνατότητας](https://docs.microsoft.com/intune/custom-notifications).
