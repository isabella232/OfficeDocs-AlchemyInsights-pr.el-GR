---
title: Αντιμετώπιση προβλημάτων συμβάντων από το ηλεκτρονικό ταχυδρομείο
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
- "9000301"
- "5765"
ms.openlocfilehash: 2cea347f248a3b04873428946f1817657af04773
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834839"
---
# <a name="troubleshooting-events-from-email"></a>Αντιμετώπιση προβλημάτων συμβάντων από το ηλεκτρονικό ταχυδρομείο

1. Βεβαιωθείτε ότι η δυνατότητα είναι ενεργοποιημένη για το γραμματοκιβώτιο: **Get-EventsFromEmailConfiguration -Identity <mailbox>**

2. Στη συνέχεια, δείτε τα αρχεία καταγραφής "Συμβάντα από ηλεκτρονικό ταχυδρομείο" **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**

3. Στα αρχεία καταγραφής "Συμβάντα από ηλεκτρονικό ταχυδρομείο", βρείτε το InternetMessageId που ταιριάζει με το στοιχείο στο γραμματοκιβώτιο.  

4. Ο "TrustScore" καθορίζει εάν το στοιχείο προστίθεται ή όχι. Τα συμβάντα θα προστεθούν μόνο εάν το TrustScore = "Αξιόπιστο".

Το TrustScore καθορίζεται από τις ιδιότητες SPF, Dkim ή Dmarc, οι οποίες βρίσκονται στην κεφαλίδα του μηνύματος.

Για να προβάλετε αυτές τις ιδιότητες:

**Outlook υπολογιστή**

- Άνοιγμα του στοιχείου
- Αρχείο -> Ιδιότητες -> Κεφαλίδες Internet

ή

**MFCMapi**

- Μετάβαση στο στοιχείο στα Εισερχόμενα
- Αναζητήστε PR_TRANSPORT_MESSAGE_HEADERS_W

Αυτές οι ιδιότητες προσδιορίζονται και καταγράφονται κατά τη μεταφορά και δρομολόγηση. Για περαιτέρω αντιμετώπιση προβλημάτων, ίσως χρειαστεί να παρακολουθήσετε την υποστήριξη μεταφοράς σχετικά με τις αποτυχίες στα SPF, DKIM και.ή DMARC.