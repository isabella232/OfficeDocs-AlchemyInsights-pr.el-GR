---
title: Δεν βρέθηκαν συνδρομές στο Κέντρο ασφαλείας
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 777fb9b09aa26d166f9971589bda464ccb90f4be
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544108"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a>Δεν βρέθηκαν συνδρομές στο Κέντρο ασφαλείας

Εάν κατά την πρόσβαση σε Κέντρο προστασίας του Microsoft Defender λάβετε ένα μήνυμα "Δεν βρέθηκαν συνδρομές", αυτό σημαίνει ότι το Azure Active Directory (AAD) που χρησιμοποιείται για τη σύνδεση του χρήστη στην πύλη δεν διαθέτει Microsoft Defender ATP άδεια χρήσης.  

Οι Windows E5 και Office E5 είναι ξεχωριστές άδειες χρήσης.

Ανοίξτε μια υπόθεση υποστήριξης εάν η άδεια χρήσης αγοράστηκε, αλλά δεν έχει γίνει προμήθεια σε αυτήν την παρουσία AAD. Είτε έχετε: <br/>
-   Ένα πιθανό πρόβλημα παροχής αδειών χρήσης.<br/>
-   Κατά λάθος, εκνεύσατε την άδεια χρήσης σε διαφορετικό Microsoft AAD από αυτό που χρησιμοποιήθηκε για τον έλεγχο ταυτότητας στην υπηρεσία.