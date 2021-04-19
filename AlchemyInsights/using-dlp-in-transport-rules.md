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
ms.openlocfilehash: e512b36b34c5fc4931fb0f796790ee4b01c6443c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827216"
---
# <a name="using-dlp-in-transport-rules"></a>Χρήση DLP στους κανόνες μεταφοράς

Για να ενσωματώσετε την αποτροπή απώλειας δεδομένων (DLP) σε μια ήδη υπάρχουσα μεταφορά, εφαρμόστε τη συνθήκη "**Εάν το μήνυμα περιέχει...Ευαίσθητες πληροφορίες**" στη ρύθμιση κανόνα μεταφοράς.

**Για περισσότερες λεπτομέρειες, ανατρέξτε στο θέμα:**

- Ενσωματωμένοι τύποι ευαίσθητων στοιχείων DLP στους κανόνες μεταφοράς: [Ενσωμάτωση κανόνων ευαίσθητων πληροφοριών](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).

Μπορείτε επίσης να ελέγξετε τον κανόνα, με ή χωρίς έλεγχο πολιτικής, κάνοντας χρήση της "λειτουργίας δοκιμής" στον κανόνα.  Θα πρέπει να περιμένετε 30 λεπτά μετά τη δημιουργία του κανόνα, για να τον ελέγξετε.

- Ανατρέξτε στο θέμα [Έλεγχος ροής αλληλογραφίας/κανόνες μεταφοράς](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)

**Σημείωση**: Εάν προσπαθείτε να εφαρμόσετε μια νέα πολιτική DLP με τους κανόνες μεταφοράς που εφαρμόζονται στην EAC, χρησιμοποιήστε αντί αυτού τις [Πολιτικές DLP του κέντρου ασφαλείας και συμμόρφωσης](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide).
