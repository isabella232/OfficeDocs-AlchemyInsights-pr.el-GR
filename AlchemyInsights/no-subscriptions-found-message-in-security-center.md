---
title: Μήνυμα "Δεν βρέθηκαν συνδρομές" στο Κέντρο ασφαλείας
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
ms.openlocfilehash: 01117bc535df14533e426fd2d31c336fccc75611
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/15/2020
ms.locfileid: "50713603"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a>Μήνυμα "Δεν βρέθηκαν συνδρομές" στο Κέντρο ασφαλείας

Αν κατά την πρόσβαση στο Κέντρο προστασίας του Microsoft Defender εμφανιστεί το μήνυμα "Δεν βρέθηκαν συνδρομές", αυτό σημαίνει ότι το Azure Active Directory (AAD) που χρησιμοποιήθηκε για τη σύνδεση του χρήστη στην πύλη δεν διαθέτει άδεια χρήσης atP του Microsoft Defender.  

Οι άδειες χρήσης των Windows E5 και Office E5 είναι ξεχωριστές άδειες χρήσης.

Ανοίξτε μια υπόθεση υποστήριξης εάν η άδεια χρήσης αγοράστηκε, αλλά δεν έχει γίνει προμήθεια σε αυτήν την παρουσία AAD. Είτε έχετε: <br/>
-   Ένα πιθανό πρόβλημα παροχής άδειας χρήσης.<br/>
-   Εκδόσατε κατά λάθος την άδεια χρήσης σε ένα διαφορετικό Microsoft AAD από αυτό που χρησιμοποιήθηκε για τον έλεγχο ταυτότητας στην υπηρεσία.