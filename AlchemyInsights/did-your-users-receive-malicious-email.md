---
title: Έλαβαν οι χρήστες σας κακόβουλα μηνύματα ηλεκτρονικού ταχυδρομείου
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
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: 2197e7f195d789193798b80cb092d8046eb6e0be
ms.sourcegitcommit: 3c708a4a349b60b59bc623c44fb78674c685f3c2
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 02/18/2021
ms.locfileid: "50291792"
---
# <a name="did-your-users-receive-malicious-email"></a>Έλαβαν οι χρήστες σας κακόβουλα μηνύματα ηλεκτρονικού ταχυδρομείου;

- Μπορείτε πλέον να αναφέρετε το κακόβουλο μήνυμα ηλεκτρονικού ταχυδρομείου στη Microsoft χρησιμοποιώντας τις [Υποβολές διαχειριστών στο κέντρο ασφάλειας και συμμόρφωσης](https://sip.protection.office.com/reportsubmission).

Τα μηνύματα που υποβάλλονται στις [Υποβολές διαχειριστών](https://sip.protection.office.com/reportsubmission) σαρώνονται και τα ακόλουθα αποτελέσματα εμφανίζονται στο αναδυόμενο μήνυμα **λεπτομέρειες**:

- Εάν υπήρξε αποτυχία στον έλεγχο ταυτότητας ηλεκτρονικού ταχυδρομείου του αποστολέα τη στιγμή της παράδοσης.
- Πληροφορίες σχετικά με τυχόν πολιτικές που θα μπορούσαν να έχουν επηρεάσει ή να παρακάμψει την κρίση ενός μηνύματος.
- Τρέχοντα αποτελέσματα αναζήτησης για να δείτε εάν οι διευθύνσεις URL ή τα αρχεία που περιέχονται στο μήνυμα ήταν κακόβουλες ή όχι.
- Σχόλια από βαθμολογητές

Εάν βρεθεί μια παράκαμψη, το νέα σάρωση θα πρέπει να ολοκληρωθεί σε αρκετά λεπτά. Εάν δεν υπάρχει πρόβλημα στον έλεγχο ταυτότητας ηλεκτρονικού ταχυδρομείου ή εάν η παράδοση δεν επηρεάζεται από μια παράκαμψη, τότε μπορεί να λάβετε τα σχόλια από τους βαθμολογητές σε έως και μία ημέρα.

Εάν διαφωνείτε με την τελική κρίση ενός μηνύματος, διεύθυνσης URL ή αρχείου (αποκλεισμένου έναντι μη αποκλεισμένου), υποβάλετε το μήνυμα ξανά μετά από μια ημέρα για νέα σάρωση. Οι πιθανότητες να αλλάξει η κρίση είναι μεγάλες μετά την εκ νέου υποβολή του μηνύματος.

Στο μεταξύ, μπορείτε να καταργήσετε κακόβουλα μηνύματα ηλεκτρονικού ταχυδρομείου από τα εισερχόμενα των χρηστών, ακολουθώντας τις οδηγίες σε[αυτό το άρθρο](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).

- Οι πελάτες που έχουν το Microsoft Defender για Office 365 μπορούν να:
    - χρησιμοποιήσουν την [Εξερεύνηση απειλών για εύρεση και διαγραφή ύποπτων μηνυμάτων ηλεκτρονικού ταχυδρομείου](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)
    - [χρησιμοποιήσουν τις Ασφαλείς συνδέσεις για τον αποκλεισμό της προσβασιμότητας](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) κακόβουλων διευθύνσεων URL
    - παρακολουθούν χρήστες που έχουν κάνει κλικ και έχουν εισέλθει σε κακόβουλες διευθύνσεις URL: [Προβολή διευθύνσεων URL ηλεκτρονικού "ψαρέματος" και κλικ σε δεδομένα κρίσεων](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)
    - [εκκινήσουν μια Αυτοματοποιημένη έρευνα](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office) χειροκίνητα

Επίσης, μπορείτε να προστατεύεστε από κακόβουλα αρχεία και διευθύνσεις URL, ακολουθώντας τις οδηγίες στο άρθρο [Προστασία από κακόβουλες διευθύνσεις URL και αρχεία](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).