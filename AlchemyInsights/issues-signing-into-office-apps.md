---
title: Θέματα είσοδο σε εφαρμογές του Office
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
ms.openlocfilehash: 5f500ecf1f779fb1be4d257fd050a3ad054087dc
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938224"
---
# <a name="fixing-the-office-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Τον καθορισμό του μηνύματος "λειτουργική μονάδα Trusted Platform του υπολογιστή σας δεν λειτουργεί σωστά" εφαρμογές Office

Για να διορθώσετε αυτό το σφάλμα, δοκιμάστε τα εξής:

- Εγκαταστήστε τις τελευταίες ενημερωμένες εκδόσεις για [Windows](https://support.microsoft.com/help/4027667/windows-10-update) και του [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Απαλοιφή Office διαπιστευτήρια](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) χρησιμοποιώντας τη Διαχείριση διαπιστευτηρίων των Windows.<br/>
    **Σημείωση:** Οι διαδρομές μητρώου για το Office 2016 έχουν αλλάξει σε 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Δοκιμάστε τη [διαδικασία αποκατάστασης του χρήστη](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) για να διορθώσετε τα σφάλματα της μονάδας αξιόπιστης πλατφόρμας (TPM).
- Ορίστε το EnableADAL = 0, ακολουθώντας τα εξής βήματα:  
    1. Κάντε δεξιό κλικ στο κουμπί Έναρξη των Windows, επιλέξτε **Εκτέλεση**, πληκτρολογήστε **regedit**και, στη συνέχεια, επιλέξτε το κουμπί **OK**.
    2. Επιλέξτε **Ναι** για να επιτρέψετε τον Επεξεργαστή μητρώου για να κάνετε αλλαγές στη συσκευή σας.
    3. Στον επεξεργαστή μητρώου, προσθέστε μια τιμή DWORD του **EnableADAL** με τη ρύθμιση **0** στην περιοχή HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Για περισσότερες πληροφορίες, ανατρέξτε στην ενότητα [ζητήματα σύνδεσης στο είσοδος μετά την ενημερωμένη έκδοση του Office 2016 build 16.0.7967 σε Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).