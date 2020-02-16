---
title: Καθορισμός των εφαρμογών του Office ο λογαριασμός σας βρίσκεται σε μήνυμα κακής κατάστασης
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: e591c56dd207a5bcb3979be3f66052121100b162
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 12/27/2019
ms.locfileid: "41969473"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a>Επιδιόρθωση των εφαρμογών του Office "ο λογαριασμός σας είναι σε κακή κατάσταση" σφάλμα

Για να διορθώσετε αυτό το σφάλμα, δοκιμάστε τις ακόλουθες επιλογές στον υπολογιστή που επηρεάζεται:

- Ανοίξτε μια εφαρμογή του Office, επιλέξτε υπογραφή**λογαριασμού** >  **αρχείου** > **από όλους τους λογαριασμούς**. Συνδεθείτε ξανά χρησιμοποιώντας ένα λογαριασμό χρήστη με έγκυρη άδεια χρήσης. Για λεπτομερείς πληροφορίες, ανατρέξτε [στο λογαριασμό λογαριασμοί στο Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Καταργήστε τις πιστοποιήσεις του Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) χρησιμοποιώντας τη Διαχείριση διαπιστευτηρίων των Windows.<br>
  **Σημείωση:** Οι διαδρομές μητρώου για το Office 2016 έχουν αλλάξει σε 16,0. Για παράδειγμα, \Software\Microsoft\Office\16.0\Common\Identity\
- Στον υπολογιστή που επηρεάζεται, ορίστε το EnableADAL = 0, ακολουθώντας τα εξής βήματα:  
     1. Κάντε δεξιό κλικ στο κουμπί των Windows και επιλέξτε **Εκτέλεση**. Με το **Άνοιγμα** πλαίσιο, πληκτρολογήστε **regedit**, και στη συνέχεια επιλέξτε **OK**.
     2. Επιλέξτε **Ναι** όταν σας ζητηθεί να επιτρέψετε στον επεξεργαστή μητρώου να κάνει αλλαγές στη συσκευή σας.
    3. Στον επεξεργαστή μητρώου, προσθέστε μια τιμή DWORD του EnableADAL με μια ρύθμιση 0 κάτω από HKEY_CURRENT_USER \Software\Microsoft\Office\16.0\Common\Identity.
- Εάν το σφάλμα παρουσιάζεται κατά τη σύνδεση με το Office 365 χρησιμοποιώντας το Office 2013, [ενεργοποιήστε τον σύγχρονο έλεγχο ταυτότητας](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) για το πρόγραμμα-πελάτη του Office.

Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Τρόπος αντιμετώπισης προβλημάτων εφαρμογών που δεν είναι προγράμματα περιήγησης που δεν είναι δυνατό να εισέλθετε στο Office 365, Azure ή Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).

