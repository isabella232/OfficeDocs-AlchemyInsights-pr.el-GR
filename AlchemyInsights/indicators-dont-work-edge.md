---
title: Οι ενδείξεις δεν λειτουργούν με το πρόγραμμα περιήγησης Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11230"
- "9005470"
ms.openlocfilehash: df62d965e0dc2ddb656571af99b1e4c3cb52ea35
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676241"
---
# <a name="indicators-dont-work-using-edge-browser"></a>Οι ενδείξεις δεν λειτουργούν με το πρόγραμμα περιήγησης Edge

Μετά τη δημιουργία μιας Ένδειξης, δεν τιμάται από τον Edge (Smartscreen). Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα Δημιουργία δεικτών για IPs και διευθύνσεις URL/τομείς.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)

## <a name="step-1-ensure-the-following"></a>Βήμα 1: Εξασφαλίστε τα εξής

- Βεβαιωθείτε ότι η ένδειξη είναι σωστή (δεν υπάρχουν λάθη στη διεύθυνση IP/URL, σωστή ενέργεια, οι σωστές ομάδες RBAC).
- Περιμένετε τουλάχιστον 2 ώρες μετά τη δημιουργία της ένδειξης για να ληφθεί υπόψη τυχόν λανθάνων χρόνος.
- Επιβεβαιώστε ότι τα συστήματα έχουν επιβεβαιωθεί στον Microsoft Defender για το τελικό σημείο.
- Βεβαιωθείτε ότι τα συστήματα μπορούν να επικοινωνούν με το Cloud.
- Βεβαιωθείτε ότι το Smartscreen είναι ενεργοποιημένο και προσβάσιμο, από την τοποθεσία [δοκιμής.](https://demo.smartscreen.msft.net)

## <a name="step-2-troubleshoot-the-potential-issue"></a>Βήμα 2: Αντιμετώπιση του πιθανού προβλήματος

- Βεβαιωθείτε ότι το πρόγραμμα-πελάτης πληροί τις απαιτήσεις. Για λεπτομέρειες, [ανατρέξτε στο θέμα Δημιουργία δεικτών για IPs και διευθύνσεις URL/τομείς.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)
- Βεβαιωθείτε ότι χρησιμοποιείτε την πιο πρόσφατη έκδοση του προγράμματος περιήγησης Edge. Για να μάθετε την πιο πρόσφατη έκδοση, [ανατρέξτε στο θέμα Μάθετε ποια έκδοση Microsoft Edge που έχετε.](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb)
- Επανεκκινήστε το πρόγραμμα περιήγησης Edge.
- Μεταβείτε στην τοποθεσία για την οποία έχετε ρυθμίσει μια ένδειξη. Εάν η τοποθεσία δεν εμφανίζεται όπως αναμένεται, συνεχίστε στο βήμα 3. 

## <a name="step-3-collect-data"></a>Βήμα 3: Συλλογή δεδομένων

- Συλλέξτε **διαγνωστικά δεδομένα MDEClientAnalyzer.** Για οδηγίες, [ανατρέξτε στο θέμα Προβλήματα με τους υπολογιστές που είναι σε θέση να ενταφιούν στον Microsoft Defender για το τελικό σημείο.](issues-with-onboarding-machines.md)
- Εάν είστε άνετα να εγκαταστήσετε και να συλλέξετε μια ανίχνευση Fiddler, [ανατρέξτε στο θέμα Telerik Fiddler.](http://www.telerik.com/fiddler)
- Εάν προτιμάτε οδηγίες από την Υποστήριξη της Microsoft, επιλέξτε το εικονίδιο υποστήριξης παρακάτω για να ανοίξετε μια υπόθεση υποστήριξης.
