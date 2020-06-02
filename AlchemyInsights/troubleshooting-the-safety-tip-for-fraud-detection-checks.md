---
title: Αντιμετώπιση προβλημάτων του άκρου ασφαλείας για ελέγχους εντοπισμού απάτης
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 74913492a086de688067d588e95dd87e6946743b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44504983"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Αντιμετώπιση προβλημάτων του άκρου ασφαλείας για ελέγχους εντοπισμού απάτης

Εάν παίρνετε μια συμβουλή ασφαλείας που λέει "Ο αποστολέας απέτυχε ελέγχους ανίχνευσης απάτης μας και δεν μπορεί να είναι αυτό που φαίνεται να είναι", τότε ο αποστολέας απέτυχε να περάσει είτε DKIM ή SPF ελέγχους ταυτότητας. Η καλύτερη μέθοδος για την επίλυση αυτού είναι ο αποστολέας να εξουσιοδοτήσει τον εαυτό του. Εάν ο αποστολέας στέλνει για λογαριασμό σας, πρέπει να τον εξουσιοδοτήσετε προσθέτοντας τη διεύθυνση IP του αποστολέα στην εγγραφή SPF.
  
Ανατρέξτε [στο θέμα Αντιμετώπιση προβλημάτων της κόκκινης (ύποπτης) συμβουλής ασφαλείας για ελέγχους εντοπισμού απάτης](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) για περισσότερες πληροφορίες.
  
Ακολουθούν ορισμένες άλλες συνδέσεις που μπορούν να σας βοηθήσουν:
  
- [Τρόπος με τον οποίο η Microsoft χρησιμοποιεί το πλαίσιο πολιτικής αποστολέα (SPF) για την αποτροπή πλαστογραφίας](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [Ρύθμιση spf για την αποτροπή πλαστοπλασιασμός](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
