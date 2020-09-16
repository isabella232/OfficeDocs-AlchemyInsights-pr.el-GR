---
title: Επιδιόρθωση των εφαρμογών του Microsoft 365 ο λογαριασμός σας βρίσκεται σε μήνυμα κακής κατάστασης
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
- "2558"
- "9000571"
ms.openlocfilehash: ec529291ec9406eba9dc2b0f2cc7a93c77fa3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744545"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a>Σφάλμα διόρθωσης των εφαρμογών Microsoft 365 "ο λογαριασμός σας βρίσκεται σε εσφαλμένη κατάσταση"

Για να διορθώσετε αυτό το σφάλμα, δοκιμάστε τις παρακάτω επιλογές στον υπολογιστή που επηρεάζεται:

- Ανοίξτε μια εφαρμογή του Office, επιλέξτε Έξοδος λογαριασμού **αρχείου**από  >  **Account**  >  **όλους τους λογαριασμούς**. Πραγματοποιήστε είσοδο ξανά χρησιμοποιώντας ένα λογαριασμό χρήστη με έγκυρη άδεια χρήσης. Για περισσότερες λεπτομέρειες, ανατρέξτε στο θέμα [Λογαριασμοί στο Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Καταργήστε τα διαπιστευτήρια του Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) χρησιμοποιώντας τη Διαχείριση διαπιστευτηρίων των Windows.<br>
  **Σημείωση:** Οι διαδρομές μητρώου για το Office 2016 έχουν αλλάξει σε 16,0. Για παράδειγμα, \Software\Microsoft\Office\16.0\Common\Identity\
- Εάν το σφάλμα εμφανίζεται κατά τη σύνδεση στο Office 365 με χρήση του Office 2013, [Ενεργοποιήστε τον σύγχρονο έλεγχο ταυτότητας](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) για το πρόγραμμα-πελάτη του Office.

Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Τρόπος αντιμετώπισης προβλημάτων εφαρμογών εκτός προγράμματος περιήγησης που δεν μπορούν να εισέλθετε στο Microsoft 365, το Azure ή το Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).

