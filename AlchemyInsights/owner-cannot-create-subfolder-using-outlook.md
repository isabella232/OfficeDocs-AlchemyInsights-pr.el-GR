---
title: Ο κάτοχος δεν μπορεί να δημιουργήσει υποφάκελο χρησιμοποιώντας Outlook
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
ms.openlocfilehash: 60190727e75c120ad3915da8b563b7f6b1a3238b46bb6e14cbf956365e1a84e0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54063124"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Ο κάτοχος δεν μπορεί να δημιουργήσει υποφάκελο χρησιμοποιώντας Outlook

**Υπάρχει ένα συνεχιζόμενο πρόβλημα με τους κατόχους δημόσιων φακέλων που δημιουργούν υποφακέλους χρησιμοποιώντας Outlook. Το πρόβλημα θα διορθωθεί σύντομα.**

Στο μεταξύ, χρησιμοποιήστε μία από τις παρακάτω λύσεις:

1. Χρησιμοποιήστε Outlook για MAC για να δημιουργήσετε τον υποφάκελο, καθώς το πρόβλημα επηρεάζει μόνο Outlook υπολογιστή windows (όλες τις εκδόσεις)
2. Να έχει ο διαχειριστής τη δημιουργία του υποφακέλου χρησιμοποιώντας το κέλυφος EXO ή το EAC
3. Αλλαγή του DefaultPublicFolderMailbox/EffectivePublicFolderMailbox στο χρήστη σε άλλο γραμματοκιβώτιο εκτός από το γραμματοκιβώτιο περιεχομένου για το φάκελο που προκαλεί το πρόβλημα  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. Περιμένετε μία ώρα, επανεκκινήστε το πρόγραμμα-πελάτη του Outlook