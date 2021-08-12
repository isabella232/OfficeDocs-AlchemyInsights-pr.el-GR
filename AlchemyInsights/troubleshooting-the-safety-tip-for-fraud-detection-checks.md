---
title: Αντιμετώπιση προβλημάτων του συμβουλή ασφαλείας για ελέγχους εντοπισμού απάτης
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: c7ee1fcc887a3221b5f2acda1aa6ae6beb03cb96686d4ecb7828a02f8ff48302
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53955966"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Αντιμετώπιση προβλημάτων του συμβουλή ασφαλείας για ελέγχους εντοπισμού απάτης

Εάν εμφανίζεται ένα μήνυμα συμβουλή ασφαλείας "Ο αποστολέας απέτυχε στους ελέγχους εντοπισμού απάτης και ενδέχεται να μην είναι αυτός που φαίνεται να είναι", τότε ο αποστολέας απέτυχε να περάσει ελέγχους ελέγχου ταυτότητας DKIM ή SPF. Η καλύτερη μέθοδος για την επίλυση αυτού του προβλήματος είναι να εξουσιοδοτήσει τον αποστολέα. Εάν ο αποστολέας στέλνει εκ μέρους σας, πρέπει να τον εξουσιοδοτήσετε προσθέτοντας τη διεύθυνση IP του αποστολέα στην εγγραφή SPF.
  
Ανατρέξτε [στο θέμα Αντιμετώπιση προβλημάτων των κόκκινων (ύποπτων) συμβουλή ασφαλείας για ελέγχους εντοπισμού απάτης](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) για περισσότερες πληροφορίες.
  
Ακολουθούν ορισμένες άλλες συνδέσεις που μπορούν να σας βοηθήσουν:
  
- [Πώς η Microsoft χρησιμοποιεί το πλαίσιο πολιτικής αποστολέα (SPF) για την αποτροπή πλαστογράφησης](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [Ρύθμιση SPF για την αποτροπή πλαστογράφησης](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
