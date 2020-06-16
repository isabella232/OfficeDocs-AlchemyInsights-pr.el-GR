---
title: Ο κάτοχος δεν είναι δυνατό να δημιουργήσει δευτερεύοντα φάκελο χρησιμοποιώντας το Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 2116bb837e4378ea29d7882df1d3010b3a4e0b1c
ms.sourcegitcommit: 936330b11fec49f6174eadea6c765bdf9e6ba784
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/12/2020
ms.locfileid: "44748907"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Ο κάτοχος δεν είναι δυνατό να δημιουργήσει δευτερεύοντα φάκελο χρησιμοποιώντας το Outlook

**Υπάρχει ένα συνεχιζόμενο ζήτημα με τους κατόχους δημόσιων φακέλων που δημιουργούν υποφακέλους χρησιμοποιώντας το Outlook. Το ζήτημα θα διορθωθεί σύντομα.**

Εν τω μεταξύ, χρησιμοποιήστε μία από τις ακόλουθες λύσεις:

1. Χρήση του Outlook για MAC για τη δημιουργία του υποφακέλου, καθώς το ζήτημα επηρεάζει μόνο το Outlook για παράθυρα επιφάνειας εργασίας (όλες οι εκδόσεις)
2. Να δημιουργήσει ο διαχειριστής τον υποφάκελο χρησιμοποιώντας το κέλυφος EXO ή την ΑΗΚ
3. Αλλαγή του πλαισίου DefaultPublicFolderMailbox/EffectivePublicFolderMailbox στο χρήστη σε άλλο γραμματοκιβώτιο από το γραμματοκιβώτιο περιεχομένου για το φάκελο που προκαλεί ζήτημα  
    - *Set-Γραμματοκιβώτιο User1 DefaultPublicFolderMailbox PubMBX3*
4. Περιμένετε για μια ώρα, κάντε επανεκκίνηση του προγράμματος-πελάτη του Outlook