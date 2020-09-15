---
title: Προβλήματα κατά την είσοδο σε εφαρμογές του Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2560"
ms.openlocfilehash: 7d2cfd437bb55804c3b9263428833c10d5caaa47
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695323"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Επιδιόρθωση των εφαρμογών του Microsoft 365 "Λυπούμαστε, ένας άλλος λογαριασμός από τον οργανισμό σας έχει ήδη εισέλθει στο" μήνυμα

Για να διορθώσετε αυτό το σφάλμα, δοκιμάστε τα εξής:

- Καταργήστε όλους τους λογαριασμούς εργασίας, εκτός από τον επηρεαζόμενο λογαριασμό, χρησιμοποιώντας τις ρυθμίσεις των Windows > την **εργασία ή το σχολείο της Access**.
- [Καταργήστε τα διαπιστευτήρια του Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) χρησιμοποιώντας τη Διαχείριση διαπιστευτηρίων των Windows.<br/>
    **Σημείωση:** Οι διαδρομές μητρώου για το Office 2016 έχουν αλλάξει σε 16,0. (Π.χ.: \Software\Microsoft\Office\16.0\Common\Identity\)
- Ανοίξτε μια εφαρμογή του Office, επιλέξτε Έξοδος λογαριασμού **αρχείου**  >  **Account**  >  **Sign Out**. Στη συνέχεια, συνδεθείτε χρησιμοποιώντας ένα λογαριασμό χρήστη με μια έγκυρη άδεια χρήσης. Για περισσότερες λεπτομέρειες, ανατρέξτε στο θέμα [Λογαριασμοί στο Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Για Mac, ανατρέξτε στο θέμα [Δεν μπορώ να συνδεθώ σε μια εφαρμογή Office 2016 για Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα "Λυπούμαστε, ένας άλλος λογαριασμός από τον οργανισμό σας έχει ήδη εισέλθει σε αυτόν τον υπολογιστή" στο Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).