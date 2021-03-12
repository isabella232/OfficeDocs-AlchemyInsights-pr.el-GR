---
title: Δεν είναι δυνατή η αποστολή/λήψη ηλεκτρονικού ταχυδρομείου από/προς το Office 365 λόγω της απενεργοποίησης TLS 1.0 και TLS 1.1
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005383"
- "9275"
ms.openlocfilehash: 9927112608ae58751e43c1bf0592fbd4a7cf1a0e
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50745018"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a>Δεν είναι δυνατή η αποστολή/λήψη ηλεκτρονικού ταχυδρομείου από/προς το Office 365 λόγω της απενεργοποίησης TLS 1.0 και TLS 1.1

Όπως επιβεβαιώθηκε από τη δημοσίευση mc229914 του κέντρου μηνυμάτων, η απόσβεση TLS 1.0 και TLS 1.1 ξεκίνησε την επιβολή για τελικά σημεία ροής αλληλογραφίας του Exchange Online. Σύντομα το Office 365 δεν θα δέχεται πλέον συνδέσεις ηλεκτρονικού ταχυδρομείου TLS 1.0 και TLS 1.1 από εξωτερικές προελεύσεις. Επίσης, το Exchange Online δεν θα χρησιμοποιεί ποτέ TLS 1.0 ή 1.1 για την αποστολή εξερχόμενων μηνυμάτων ηλεκτρονικού ταχυδρομείου. Εάν αντιμετωπίζετε προβλήματα λόγω απενεργοποίησης TLS 1.0 ή 1.1, ενδέχεται να αντιμετωπίσετε ένα από τα ακόλουθα σφάλματα.

- Ο αποστολέας επιστρέφει την επιστροφή NDR - "421 4.4.2 Η σύνδεση απορρίφθηκε λόγω SocketError"
- Σφάλμα στο πρόγραμμα προβολής ουράς του διακομιστή εσωτερικής εγκατάστασης που στέλνει μηνύματα ηλεκτρονικού ταχυδρομείου στον Υπεύθυνο 365- '421 4.4.2 Η σύνδεση απορρίφθηκε λόγω SocketError'
- Σφάλμα στο αρχείο καταγραφής "Αποστολή πρωτοκόλλου [σύνδεσης"](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) στο διακομιστή που στέλνει μηνύματα ηλεκτρονικού ταχυδρομείου στο Office 365- Η διαπραγμάτευση TLS απέτυχε με σφάλμα SocketError
- Σφάλμα στο αρχείο καταγραφής πρωτοκόλλου αποστολής ή λήψης σύνδεσης - "451 5.7.3 Πρέπει πρώτα να εκδώσει μια εντολή STARTTLS"

Εάν αντιμετωπίσετε οποιοδήποτε από τα παραπάνω σφάλματα, βεβαιωθείτε ότι ο διακομιστής που στέλνει ή λαμβάνει μηνύματα ηλεκτρονικού ταχυδρομείου έχει ενεργοποιημένο το TLS 1.2, ελέγχοντας τα ακόλουθα κλειδιά μητρώου.

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2\Πρόγραμμα-πελάτης] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**

Εάν κάνετε οποιαδήποτε αλλαγή στα παραπάνω κλειδιά μητρώου για να ενεργοποιήσετε το TLS 1.2, επανεκκινήστε το διακομιστή για να εφαρμοστούν οι αλλαγές. Επίσης, βεβαιωθείτε ότι έχετε εγκαταστήσει τις πιο πρόσφατες ενημερώσεις των Windows και του Exchange.

Για περισσότερες πληροφορίες, ανατρέξτε στα θέματα:

- [Οδηγίες TLS του Exchange Server, μέρος 1: Ετοιμάζομαι για το TLS 1.2 - Κοινότητα τεχνικής υποστήριξης της Microsoft](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [Τμήμα καθοδήγησης TLS του Exchange Server 2: Ενεργοποίηση του TLS 1.2 και προσδιορισμός των πελατών που δεν το χρησιμοποιούν - Κοινότητα τεχνικής υποστήριξης της Microsoft](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [Κατανόηση των σεναρίων ηλεκτρονικού ταχυδρομείου εάν δεν είναι δυνατή η συμφωνία εκδόσεων TLS με το Exchange Online - Κοινότητα τεχνικής υποστήριξης της Microsoft](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
