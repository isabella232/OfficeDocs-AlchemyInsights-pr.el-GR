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
ms.openlocfilehash: 06ded694893c020f862864215700853b19d35f08
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820178"
---
# <a name="blocking-legacy-authentication"></a>Αποκλεισμός ελέγχου ταυτότητας παλαιού τύπου

Ο έλεγχος ταυτότητας παλαιού τύπου είναι ένας όρος που αναφέρεται σε μια αίτηση ελέγχου ταυτότητας που έχει γίνει από:

- Παλαιότερα προγράμματα-πελάτες του Office που δεν χρησιμοποιούν σύγχρονο έλεγχο ταυτότητας (για παράδειγμα, πρόγραμμα-πελάτη του Office 2010).

- Κάθε πρόγραμμα-πελάτης που χρησιμοποιεί πρωτόκολλα αλληλογραφίας παλαιού τύπου, όπως IMAP/SMTP/POP3.

Για περισσότερες πληροφορίες σχετικά με τον αποκλεισμό του ελέγχου ταυτότητας παλαιού τύπου και την ενεργοποίηση του σύγχρονου ελέγχου ταυτότητας, ανατρέξτε στην επιλογή [Αποκλεισμός ελέγχου ταυτότητας παλαιού τύπου.](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication)

Οι προεπιλογές ασφαλείας στο Azure Active Directory (Azure AD) διευκολύνουν την ασφάλεια και την προστασία του οργανισμού σας. Οι προεπιλογές ασφαλείας περιέχουν προκαθορισμένες ρυθμίσεις ασφαλείας για συνηθισμένες επιθέσεις.
Για περισσότερες πληροφορίες σχετικά με τις προεπιλογές ασφαλείας, ανατρέξτε στο [θέμα Τι είναι οι προεπιλογές ασφαλείας;](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults). 

**Σημείωση:** Εάν ο μισθωτής σας δημιουργήθηκε στις ή μετά τις 22 Οκτωβρίου 2019, είναι πιθανό να αντιμετωπίζετε τη νέα συμπεριφορά ασφαλείας από προεπιλογή και να έχετε ήδη ενεργοποιημένες τις προεπιλογές ασφαλείας στο μισθωτή σας.  Σε μια προσπάθεια να προστατεύσουμε όλους τους χρήστες μας, οι προεπιλογές ασφαλείας επιτρέπουν τη δημιουργία όλων των νέων μισθωτών.
