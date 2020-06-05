---
title: Ζητήματα που σχετίζονται με την είσοδο στο Microsoft 365 εφαρμογές
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: 4e7612562d036f1c717817d3c883d6df80f86e2f
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579865"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Επιδιόρθωση του μηνύματος "Η μονάδα αξιόπιστης πλατφόρμας του υπολογιστή σας δεν λειτουργεί σωστά"

Για να διορθώσετε αυτό το σφάλμα, δοκιμάστε τα εξής:

- Εγκαταστήστε τις πιο πρόσφατες ενημερωμένες εκδόσεις για [τα Windows](https://support.microsoft.com/help/4027667/windows-10-update) και [το Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Καταργήστε τις πιστοποιήσεις του Office χρησιμοποιώντας](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) τη Διαχείριση διαπιστευτηρίων των Windows.<br/>
    **Σημείωση:** Οι διαδρομές μητρώου για το Office 2016 έχουν αλλάξει σε 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Δοκιμάστε τη [διαδικασία αποκατάστασης χρήστη](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) για να διορθώσετε αποτυχίες λειτουργικής μονάδας αξιόπιστης πλατφόρμας (TPM).
- Ορίστε το EnableADAL = 0 χρησιμοποιώντας τα ακόλουθα βήματα:  
    1. Κάντε δεξί κλικ στο κουμπί "Έναρξη των Windows", επιλέξτε **"Εκτέλεση",** πληκτρολογήστε **regedit**και, στη συνέχεια, επιλέξτε **OK**.
    2. Επιλέξτε **Ναι** για να επιτρέψετε στον Επεξεργαστή Μητρώου (Registry Editor) να κάνει αλλαγές στη συσκευή σας.
    3. Στον Επεξεργαστή Μητρώου ( Registry Editor), προσθέστε μια τιμή DWORD του **EnableADAL** με ρύθμιση **0** κάτω από HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Ζητήματα σύνδεσης κατά την είσοδο μετά την ενημέρωση για τη δημιουργία του Office 2016 16.0.7967 στα Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).