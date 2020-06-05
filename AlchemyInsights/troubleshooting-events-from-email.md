---
title: Αντιμετώπιση προβλημάτων συμβάντων από ηλεκτρονικό ταχυδρομείο
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: e27589b7f6730036040b948b6275cef072fd8235
ms.sourcegitcommit: dc149ab45fbc2c974b54fb81156d2bc1b07017bb
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44569142"
---
# <a name="troubleshooting-events-from-email"></a>Αντιμετώπιση προβλημάτων συμβάντων από ηλεκτρονικό ταχυδρομείο

1. Επαλήθευση της δυνατότητας είναι ενεργοποιημένη για το γραμματοκιβώτιο: **Get-EventsFromEmailConfiguration -Ταυτότητα <mailbox> **

2. Στη συνέχεια, κοιτάξτε τα αρχεία καταγραφής "Συμβάντα από ηλεκτρονικό ταχυδρομείο" **"Εξαγωγή-ΓραμματοκιβώτιοΔιαγνωστικά <mailbox> Logs-Προφίλ χρόνου στοιχείου"**

3. Στα αρχεία καταγραφής "Συμβάντα από ηλεκτρονικό ταχυδρομείο", βρείτε το InternetMessageId που ταιριάζει με το στοιχείο στο γραμματοκιβώτιο.  

4. Το TrustScore καθορίζει εάν το στοιχείο έχει προστεθεί ή όχι. Τα συμβάντα θα προστεθούν μόνο αν το TrustScore = "Αξιόπιστο".

Το TrustScore καθορίζεται από τις ιδιότητες SPF, Dkim ή Dmarc, οι οποίες βρίσκονται στην κεφαλίδα μηνύματος.

Για να προβάλετε αυτές τις ιδιότητες:

**Επιφάνεια εργασίας outlook**

- Άνοιγμα του στοιχείου
- Αρχείο -ιδιότητες > -> κεφαλίδες Internet

Ή

**Mfcmapi**

- Μετάβαση στο στοιχείο στα εισερχόμενα
- Ψάξτε για PR_TRANSPORT_MESSAGE_HEADERS_W

Αυτές οι ιδιότητες προσδιορίζονται και καταγράφονται κατά τη μεταφορά και τη δρομολόγηση. Για περαιτέρω αντιμετώπιση προβλημάτων, ίσως χρειαστεί να παρακολουθήσετε με την Υποστήριξη μεταφορών σχετικά με τις αποτυχίες σε SPF, DKIM και.or DMARC.