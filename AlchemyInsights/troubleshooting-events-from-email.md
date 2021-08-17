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
ms.openlocfilehash: b6a8b2a1174f04a1e0ed0fdee9a954bb3bf108038f0804353d84755e490f5f47
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105352"
---
# <a name="troubleshooting-events-from-email"></a>Αντιμετώπιση προβλημάτων συμβάντων από το ηλεκτρονικό ταχυδρομείο

1. Βεβαιωθείτε ότι η δυνατότητα είναι ενεργοποιημένη για το γραμματοκιβώτιο: **Get-EventsFromEmailConfiguration -Identity <mailbox>**

2. Στη συνέχεια, δείτε τα αρχεία καταγραφής "Συμβάντα από ηλεκτρονικό ταχυδρομείο" **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**

3. Στα αρχεία καταγραφής "Συμβάντα από ηλεκτρονικό ταχυδρομείο", βρείτε το InternetMessageId που ταιριάζει με το στοιχείο στο γραμματοκιβώτιο.  

4. Ο "TrustScore" καθορίζει εάν το στοιχείο προστίθεται ή όχι. Τα συμβάντα θα προστεθούν μόνο εάν το TrustScore = "Αξιόπιστο".

Το TrustScore καθορίζεται από τις ιδιότητες SPF, Dkim ή Dmarc, οι οποίες βρίσκονται στην κεφαλίδα του μηνύματος.

Για να προβάλετε αυτές τις ιδιότητες:

**Desktop Outlook**

- Άνοιγμα του στοιχείου
- Αρχείο -> Ιδιότητες -> Κεφαλίδες Internet

ή

**MFCMapi**

- Μετάβαση στο στοιχείο στα Εισερχόμενα
- Αναζητήστε PR_TRANSPORT_MESSAGE_HEADERS_W

Αυτές οι ιδιότητες προσδιορίζονται και καταγράφονται κατά τη μεταφορά και δρομολόγηση. Για περαιτέρω αντιμετώπιση προβλημάτων, ίσως χρειαστεί να παρακολουθήσετε την υποστήριξη μεταφοράς σχετικά με τις αποτυχίες στα SPF, DKIM και.ή DMARC.