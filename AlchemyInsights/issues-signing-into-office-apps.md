---
title: Προβλήματα κατά την είσοδο σε εφαρμογές του Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: c64cf2c9dbf63caad22e54ae801adc3ed8ff0f62
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833003"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Επιδιόρθωση των εφαρμογών microsoft 365 "Η λειτουργική μονάδα αξιόπιστης πλατφόρμας του υπολογιστή σας δεν λειτουργεί σωστά"

Για να διορθώσετε αυτό το σφάλμα, δοκιμάστε τα εξής:

- Εγκαταστήστε τις πιο πρόσφατες ενημερώσεις για [τα Windows](https://support.microsoft.com/help/4027667/windows-10-update) και [το Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- [Καταργήστε τα διαπιστευτήρια του Office χρησιμοποιώντας](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) τη Διαχείριση διαπιστευτηρίων των Windows.<br/>
    **Σημείωση:** Οι διαδρομές μητρώου για το Office 2016 έχουν αλλάξει σε 16.0. (Π.χ.: \Software\Microsoft\Office\16.0\Common\Identity\)
- Δοκιμάστε τη διαδικασία [αποκατάστασης χρήστη για](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) να διορθώσετε αποτυχίες λειτουργικής μονάδας αξιόπιστης πλατφόρμας (TPM).
- Ορίστε το EnableADAL = 0 ακολουθώντας τα παρακάτω βήματα:  
    1. Κάντε δεξί κλικ στο κουμπί "Έναρξη των Windows", επιλέξτε **"Εκτέλεση",** πληκτρολογήστε **regedit και,** στη συνέχεια, **επιλέξτε OK.**
    2. Επιλέξτε **"Ναι"** για να επιτρέψετε στον Επεξεργαστή Μητρώου να κάνει αλλαγές στη συσκευή σας.
    3. Στον Επεξεργαστή Μητρώου, προσθέστε μια τιμή DWORD **της EnableADAL** με ρύθμιση **0** στην περιοχή HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα Προβλήματα σύνδεσης κατά την είσοδο μετά την ενημέρωση στη δόμηση [16.0.7967 του Office 2016 στα Windows 10.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)