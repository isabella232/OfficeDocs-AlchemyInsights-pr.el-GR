---
title: Χρήση DLP στους κανόνες μεταφοράς
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: ebc0fb718eb0572e849c5d780977deaee480a00c2825c18a12e4d2212342f17a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54084094"
---
# <a name="using-dlp-in-transport-rules"></a>Χρήση DLP στους κανόνες μεταφοράς

Για να ενσωματώσετε την αποτροπή απώλειας δεδομένων (DLP) σε μια ήδη υπάρχουσα μεταφορά, εφαρμόστε τη συνθήκη "**Εάν το μήνυμα περιέχει...Ευαίσθητες πληροφορίες**" στη ρύθμιση κανόνα μεταφοράς.

**Για περισσότερες λεπτομέρειες, ανατρέξτε στο θέμα:**

- Ενσωματωμένοι τύποι ευαίσθητων στοιχείων DLP στους κανόνες μεταφοράς: [Ενσωμάτωση κανόνων ευαίσθητων πληροφοριών](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).

Μπορείτε επίσης να ελέγξετε τον κανόνα, με ή χωρίς έλεγχο πολιτικής, κάνοντας χρήση της "λειτουργίας δοκιμής" στον κανόνα.  Θα πρέπει να περιμένετε 30 λεπτά μετά τη δημιουργία του κανόνα, για να τον ελέγξετε.

- Ανατρέξτε στο θέμα [Έλεγχος ροής αλληλογραφίας/κανόνες μεταφοράς](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)

**Σημείωση**: Εάν προσπαθείτε να εφαρμόσετε μια νέα πολιτική DLP με τους κανόνες μεταφοράς που εφαρμόζονται στην EAC, χρησιμοποιήστε αντί αυτού τις [Πολιτικές DLP του κέντρου ασφαλείας και συμμόρφωσης](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide).
