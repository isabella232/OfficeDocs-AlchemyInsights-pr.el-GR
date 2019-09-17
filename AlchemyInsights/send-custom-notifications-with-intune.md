---
title: Αποστολή προσαρμοσμένων ειδοποιήσεων με το Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.date: 07/31/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000679
ms.openlocfilehash: 1244f07fd56cf603280f1710520a04d579224e44
ms.sourcegitcommit: 16f08d051afca3c6d0de32826324f91cf63ab5ba
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/16/2019
ms.locfileid: "36992313"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Πώς να στείλετε προσαρμοσμένες ειδοποιήσεις στους χρήστες των διαχειριζόμενων συσκευών iOS και Android

Οι προσαρμοσμένες ειδοποιήσεις για το Intune υποβάλλονται σε επεξεργασία από την εφαρμογή πύλης εταιρείας στη συσκευή ενός χρήστη. Στη συνέχεια, η εφαρμογή δημιουργεί την ειδοποίηση push σε αυτήν τη συσκευή.

Τα παρακάτω είναι προαπαιτούμενα συσκευών για την υποστήριξη παραλαβής προσαρμοσμένων ειδοποιήσεων και για την εφαρμογή στη συνέχεια να δημιουργήσετε την ειδοποίηση push:

- Η συσκευή πρέπει να έχει εγκατεστημένη την εφαρμογή πύλης εταιρείας.  

- Η συσκευή πρέπει να επιτρέπει στην εφαρμογή πύλης εταιρείας να αποστέλλει ειδοποιήσεις push. Όταν η εφαρμογή έχει εγκατασταθεί ή ενημερωθεί, θα ζητήσει από το χρήστη να επιτρέψει τις ειδοποιήσεις.

- Οι συσκευές Android πρέπει να έχουν εγκατεστημένες τις υπηρεσίες Google Play.

- Η συσκευή πρέπει να εγγραφεί στο Intune.

Για περισσότερες πληροφορίες, όπως πώς να στείλετε ένα μήνυμα, ανατρέξτε στην [τεκμηρίωση της δυνατότητας](https://docs.microsoft.com/intune/custom-notifications).
