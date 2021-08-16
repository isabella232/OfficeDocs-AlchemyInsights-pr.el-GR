---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: c2f2a0c3888920a969a6fc70af7ef7bfd8435bdcf975e0f31452b5da85e3a208
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53968881"
---
# <a name="blocking-legacy-authentication"></a>Αποκλεισμός ελέγχου ταυτότητας παλαιού τύπου

Ο έλεγχος ταυτότητας παλαιού τύπου είναι ένας όρος που αναφέρεται σε μια αίτηση ελέγχου ταυτότητας που έχει γίνει από:

- Παλαιότερα Office προγράμματα-πελάτες που δεν χρησιμοποιούν σύγχρονο έλεγχο ταυτότητας (για παράδειγμα, Office πρόγραμμα-πελάτη 2010).

- Κάθε πρόγραμμα-πελάτης που χρησιμοποιεί πρωτόκολλα αλληλογραφίας παλαιού τύπου, όπως IMAP/SMTP/POP3.

Για περισσότερες πληροφορίες σχετικά με τον αποκλεισμό του ελέγχου ταυτότητας παλαιού τύπου και την ενεργοποίηση του σύγχρονου ελέγχου ταυτότητας, ανατρέξτε στην επιλογή [Αποκλεισμός ελέγχου ταυτότητας παλαιού τύπου.](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication)

Οι προεπιλογές ασφαλείας στο Azure Active Directory (Azure AD) διευκολύνουν την ασφάλεια και την προστασία του οργανισμού σας. Οι προεπιλογές ασφαλείας περιέχουν προκαθορισμένες ρυθμίσεις ασφαλείας για συνηθισμένες επιθέσεις.
Για περισσότερες πληροφορίες σχετικά με τις προεπιλογές ασφαλείας, ανατρέξτε στο [θέμα Τι είναι οι προεπιλογές ασφαλείας;](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults). 

**Σημείωση:** Εάν ο μισθωτής σας δημιουργήθηκε στις ή μετά τις 22 Οκτωβρίου 2019, είναι πιθανό να αντιμετωπίζετε τη νέα συμπεριφορά ασφαλείας από προεπιλογή και να έχετε ήδη ενεργοποιημένες τις προεπιλογές ασφαλείας στο μισθωτή σας.  Σε μια προσπάθεια να προστατεύσουμε όλους τους χρήστες μας, οι προεπιλογές ασφαλείας επιτρέπουν τη δημιουργία όλων των νέων μισθωτών.
