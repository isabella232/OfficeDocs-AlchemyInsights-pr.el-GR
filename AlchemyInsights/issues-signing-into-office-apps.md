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
- "2559"
ms.openlocfilehash: 57a4df23dc66eaf4c283dde741be6f415939633d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695179"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Μήνυμα για τη διόρθωση των εφαρμογών Microsoft 365 "η μονάδα αξιόπιστης πλατφόρμας του υπολογιστή σας δεν λειτουργεί σωστά"

Για να διορθώσετε αυτό το σφάλμα, δοκιμάστε τα εξής:

- Εγκαταστήστε τις πιο πρόσφατες ενημερώσεις για [τα Windows](https://support.microsoft.com/help/4027667/windows-10-update) και το [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Καταργήστε τα διαπιστευτήρια του Office](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) χρησιμοποιώντας τη Διαχείριση διαπιστευτηρίων των Windows.<br/>
    **Σημείωση:** Οι διαδρομές μητρώου για το Office 2016 έχουν αλλάξει σε 16,0. (Π.χ.: \Software\Microsoft\Office\16.0\Common\Identity\)
- Δοκιμάστε τη [διαδικασία αποκατάστασης χρήστη](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) για να διορθώσετε αποτυχίες της μονάδας αξιόπιστης ΠΛΑΤΦΌΡΜΑς (TPM).
- Ορίστε το EnableADAL = 0 ακολουθώντας τα παρακάτω βήματα:  
    1. Κάντε δεξί κλικ στο κουμπί Έναρξη των Windows, επιλέξτε **εκτέλεση**, πληκτρολογήστε **regedit**και, στη συνέχεια, επιλέξτε **OK**.
    2. Επιλέξτε **Ναι** για να επιτρέψετε στον επεξεργαστή μητρώου να κάνει αλλαγές στη συσκευή σας.
    3. Στον επεξεργαστή μητρώου, προσθέστε μια τιμή DWORD του **EnableADAL** με μια ρύθμιση **0** στην περιοχή HKEY_CURRENT_USER \software\microsoft\office\16.0\common\identity.

Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα προβλήματα σύνδεσης στην είσοδο μετά την ενημέρωση στο Office 2016 Δόμηση 16.0.7967 στα Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).