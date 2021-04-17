---
title: Ο κάτοχος δεν μπορεί να δημιουργήσει υποφάκελο χρησιμοποιώντας το Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: b2ab7b60bc521fd28d68333bb963528f7b9e05f2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836135"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Ο κάτοχος δεν μπορεί να δημιουργήσει υποφάκελο χρησιμοποιώντας το Outlook

**Υπάρχει ένα συνεχιζόμενο πρόβλημα με τους κατόχους δημόσιων φακέλων που δημιουργούν υποφακέλους χρησιμοποιώντας το Outlook. Το πρόβλημα θα διορθωθεί σύντομα.**

Στο μεταξύ, χρησιμοποιήστε μία από τις παρακάτω λύσεις:

1. Χρησιμοποιήστε το Outlook για MAC για να δημιουργήσετε τον υποφάκελο, καθώς το πρόβλημα επηρεάζει μόνο το Outlook για windows για υπολογιστή (όλες οι εκδόσεις)
2. Να έχει ο διαχειριστής τη δημιουργία του υποφακέλου χρησιμοποιώντας το κέλυφος EXO ή το EAC
3. Αλλαγή του DefaultPublicFolderMailbox/EffectivePublicFolderMailbox στο χρήστη σε άλλο γραμματοκιβώτιο εκτός από το γραμματοκιβώτιο περιεχομένου για το φάκελο που προκαλεί το πρόβλημα  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. Περιμένετε μία ώρα, επανεκκινήστε το πρόγραμμα-πελάτη του Outlook