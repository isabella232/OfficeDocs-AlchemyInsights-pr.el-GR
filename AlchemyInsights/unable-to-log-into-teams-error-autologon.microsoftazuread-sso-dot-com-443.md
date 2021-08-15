---
title: Δεν είναι δυνατή η σύνδεση στo Τεαμσ λόγω σφάλματος autologon.microsoftazuread-sso.com:443
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 6671a63d97f24fadc9b34907d75600a3c0ad1c9990a4a8f8d32034c11e8a952e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038400"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a>Δεν είναι δυνατή η σύνδεση στo Teams λόγω σφάλματος autologon.microsoftazuread-sso dot com:443

Εάν είναι ενεργοποιημένη η ομαλή SSO ως έλεγχος ταυτότητας O365, η διεύθυνση URL "autologon.microsoftazuread-sso.com" μπορεί να χρειαστεί να προστεθεί σε τοποθεσίες intranet.  Εάν έχει προστεθεί στο παρελθόν σε αξιόπιστες τοποθεσίες και η ομαλή SSO χρησιμοποιείται, θα πρέπει να καταργηθεί από αξιόπιστες τοποθεσίες.

Ανατρέξτε στο θέμα [Λίστα ελέγχου αντιμετώπισης προβλημάτων ομαλής SSO](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).

Ακολουθήστε τα παρακάτω βήματα για να προσθέσετε μια διεύθυνση URL στη λίστα τοποθεσίων Intranet:

1. Ανοίξτε τον Internet Explorer κάνοντας κλικ στο κουμπί **Έναρξη**. Στο πλαίσιο αναζήτησης, πληκτρολογήστε Internet Explorer και, στη συνέχεια, στη λίστα αποτελεσμάτων, κάντε κλικ στην επιλογή **Internet Explorer**.
2. Κάντε κλικ στο κουμπί **Εργαλεία** και, στη συνέχεια, κάντε κλικ στο στοιχείο **Επιλογές Internet**.
3. Κάντε κλικ στην καρτέλα **Ασφάλεια**.
4. Τώρα, κάντε κλικ στις Τοποθεσίες τοπικού intranet και, στη συνέχεια, κάντε κλικ στο κουμπί τοποθεσίες και, στη συνέχεια, στο κουμπί **Για προχωρημένους.
5. Πληκτρολογήστε τη διεύθυνση URL της τοποθεσίας Web και κάντε κλικ στην επιλογή **Προσθήκη**.
6. Όταν τελειώσετε, κάντε κλικ στην επιλογή **Κλείσιμο**.

Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Τεκμηρίωση για την ανάπτυξη ομαλής SSO για το O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (περιλαμβάνει διαδικασία που βασίζεται σε πολιτική για την προσθήκη μιας διεύθυνσης URL σε τοποθεσίες intranet στο βήμα 3).
