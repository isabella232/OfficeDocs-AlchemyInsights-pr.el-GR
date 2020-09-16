---
title: Αντιμετώπιση προβλημάτων συμβάντων από το ηλεκτρονικό ταχυδρομείο
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 9efd969e3e639c2679b0768c4a0fd045916b00d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658734"
---
# <a name="troubleshooting-events-from-email"></a>Αντιμετώπιση προβλημάτων συμβάντων από το ηλεκτρονικό ταχυδρομείο

1. Επαλήθευση ότι η δυνατότητα είναι ενεργοποιημένη για το γραμματοκιβώτιο: **Get-EventsFromEmailConfiguration- <mailbox> Identity**

2. Στη συνέχεια, δείτε τα "συμβάντα από το ηλεκτρονικό ταχυδρομείο" logs **export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**

3. Στα αρχεία καταγραφής "συμβάντα από το ηλεκτρονικό ταχυδρομείο", εντοπίστε το InternetMessageId που ταιριάζει με το στοιχείο στο γραμματοκιβώτιο.  

4. Το TrustScore προσδιορίζει εάν το στοιχείο προστίθεται ή όχι. Τα συμβάντα θα προστεθούν μόνο εάν το TrustScore = "αξιόπιστες".

Το TrustScore καθορίζεται από τις ιδιότητες SPF, DKIM ή DMARC, οι οποίες βρίσκονται στην κεφαλίδα του μηνύματος.

Για να προβάλετε αυτές τις ιδιότητες:

**Outlook υπολογιστή**

- Άνοιγμα του στοιχείου
- Ιδιότητες αρχείου->-> κεφαλίδες Internet

ή

**MFCMapi**

- Μετάβαση στο στοιχείο στο φάκελο "Εισερχόμενα"
- Αναζητήστε PR_TRANSPORT_MESSAGE_HEADERS_W

Αυτές οι ιδιότητες καθορίζονται και καταγράφονται κατά τη μεταφορά και τη δρομολόγηση. Για περαιτέρω αντιμετώπιση προβλημάτων, ίσως χρειαστεί να παρακολουθήσετε με την υποστήριξη μεταφορών τις αποτυχίες στο θέμα SPF, DKIM και. ή DMARC.