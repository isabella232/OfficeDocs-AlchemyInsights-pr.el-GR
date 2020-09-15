---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: baf3ee808cce1e4da362dd0841c0138d7d9268d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685598"
---
# <a name="blocking-legacy-authentication"></a>Αποκλεισμός παλαιού ελέγχου ταυτότητας

Ο έλεγχος ταυτότητας παλαιού τύπου είναι ένας όρος που αναφέρεται σε μια αίτηση ελέγχου ταυτότητας που γίνεται από:

- Παλαιότερα προγράμματα-πελάτες του Office που δεν χρησιμοποιούν σύγχρονο έλεγχο ταυτότητας (για παράδειγμα, πρόγραμμα-πελάτης του Office 2010).

- Οποιοσδήποτε υπολογιστής-πελάτης που χρησιμοποιεί πρωτόκολλα αλληλογραφίας παλαιού τύπου, όπως IMAP/SMTP/POP3.

Για περισσότερες πληροφορίες σχετικά με τον αποκλεισμό παλαιού ελέγχου ταυτότητας και την ενεργοποίηση του σύγχρονου ελέγχου ταυτότητας, ανατρέξτε στο θέμα [Αποκλεισμός ελέγχου ταυτότητας παλαιού τύπου](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication)

Οι προεπιλογές ασφαλείας στο Azure Active Directory (Azure AD) διευκολύνουν την ασφάλειά σας και συμβάλλουν στην προστασία του οργανισμού σας. Οι προεπιλογές ασφαλείας περιέχουν προκαθορισμένες ρυθμίσεις ασφαλείας για συνηθισμένες επιθέσεις.
Για περισσότερες πληροφορίες σχετικά με τις προεπιλογές ασφαλείας, ανατρέξτε στο θέμα [Τι είναι οι προεπιλογές ασφαλείας;](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults). 

**Σημείωση**: Εάν ο ενοικιαστής σας δημιουργήθηκε στις ή μετά τις 22 Οκτωβρίου 2019, είναι πιθανό να αντιμετωπίζετε τη νέα συμπεριφορά ασφαλούς από προεπιλογή και να έχετε ήδη ενεργοποιημένες τις προεπιλογές ασφαλείας στον μισθωτή σας.  Σε μια προσπάθεια για την προστασία όλων των χρηστών μας, οι προεπιλογές ασφαλείας εκσύρονται σε όλους τους νέους μισθωτές που δημιουργήθηκαν.
