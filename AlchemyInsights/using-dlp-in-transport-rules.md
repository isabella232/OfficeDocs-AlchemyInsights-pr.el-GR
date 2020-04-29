---
title: Χρήση DLP στους κανόνες μεταφοράς
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: 124b031e2e029b745c66a71f681f57134739eafe
ms.sourcegitcommit: 07725fcaf073f0ac145f98653b989afdb34c5ad0
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 04/28/2020
ms.locfileid: "43915180"
---
# <a name="using-dlp-in-transport-rules"></a>Χρήση DLP στους κανόνες μεταφοράς

Για να ενσωματώσετε την αποτροπή απώλειας δεδομένων (DLP) σε μια ήδη υπάρχουσα μεταφορά, εφαρμόστε τη συνθήκη "**Εάν το μήνυμα περιέχει...Ευαίσθητες πληροφορίες**" στη ρύθμιση κανόνα μεταφοράς.

**Για περισσότερες λεπτομέρειες, ανατρέξτε στο θέμα:**

- Ενσωματωμένοι τύποι ευαίσθητων στοιχείων DLP στους κανόνες μεταφοράς: [Ενσωμάτωση κανόνων ευαίσθητων πληροφοριών](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).

Μπορείτε επίσης να ελέγξετε τον κανόνα, με ή χωρίς έλεγχο πολιτικής, κάνοντας χρήση της "λειτουργίας δοκιμής" στον κανόνα.  Θα πρέπει να περιμένετε 30 λεπτά μετά τη δημιουργία του κανόνα, για να τον ελέγξετε.

- Ανατρέξτε στο θέμα [Έλεγχος ροής αλληλογραφίας/κανόνες μεταφοράς](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)

**Σημείωση**: Εάν προσπαθείτε να εφαρμόσετε μια νέα πολιτική DLP με τους κανόνες μεταφοράς που εφαρμόζονται στην EAC, χρησιμοποιήστε αντί αυτού τις [Πολιτικές DLP του κέντρου ασφαλείας και συμμόρφωσης](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide).
