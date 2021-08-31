---
title: Προβλήματα εισόδου σε εφαρμογές Microsoft 365
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
- "2574"
ms.openlocfilehash: f8f2824cc4a575ab7d7c9adec5b75e5955ec9fb5
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744636"
---
# <a name="issues-signing-into-microsoft-365-apps"></a>Προβλήματα εισόδου στο Εφαρμογές Microsoft 365

Σημείωση: Εάν χρησιμοποιείτε μια παλαιότερη έκδοση του Windows (π.χ. Windows 7 SP1, Windows Server 2008 R2), χρησιμοποιήστε την [εύκολη επιδιόρθωση](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) για να ενεργοποιήσετε το TLS 1.2 ως προεπιλογή. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα Ενημέρωση για την ενεργοποίηση των [TLS 1.1 και TLS 1.2 ως προεπιλεγμένων ασφαλών πρωτοκόλλων στο WinHTTP στο Windows.](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Για να διορθώσετε προβλήματα εισόδου με Microsoft 365 εφαρμογές, δοκιμάστε τις παρακάτω επιλογές στον υπολογιστή που επηρεάζεται:  

- Για Windows, ανατρέξτε [Προτάσεις σχετικά με την επίλυση συνηθισμένων προβλημάτων εισόδου](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues)
- Για Mac, ανατρέξτε στο θέμα Δεν είναι δυνατή η [είσοδος σε μια εφαρμογή Office 2016 για Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)

**Συμβουλή** Σε υπολογιστές με Windows, μπορούμε να διαγνώσουμε και να διορθώσουμε αυτόματα αρκετά κοινά προβλήματα εισόδου του Office για εσάς. Κατεβάστε και εκτελέστε τον **[Βοηθό υποστήριξης και αποκατάστασης για το Office 365](https://aka.ms/SaRA-OfficeSignInScenario)** για να χρησιμοποιήσετε το αυτοματοποιημένο εργαλείο μας.

**Σημείωση:**  **Δεν συνιστάται η** απενεργοποίηση του σύγχρονου ελέγχου ταυτότητας (ADAL) ή της Διαχείρισης λογαριασμού Web (WAM) για τη διόρθωση προβλημάτων εισόδου ή ενεργοποίησης. Εάν τα σφάλματα παρουσιάζονται κατά τη σύνδεση με Microsoft 365 χρησιμοποιώντας το Office 2013, βεβαιωθείτε ότι έχετε [ενεργοποιήσει τον σύγχρονο έλεγχο ταυτότητας](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) για το πρόγραμμα-πελάτη Office.

Για συγκεκριμένες ενέργειες αντιμετώπισης προβλημάτων, ανατρέξτε στα θέματα:

[Προβλήματα σύνδεσης κατά την είσοδο μετά την ενημέρωση στην έκδοση 16.0.7967 Office 2016 στο Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)  

[Δεν μπορείτε να πραγματοποιήσετε είσοδο στον εταιρικό λογαριασμό σας, όπως Office 365, Azure ή Intune](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)

[Τρόπος αντιμετώπισης προβλημάτων με εφαρμογές που δεν είναι δυνατό να πραγματοποιήσουν είσοδο στο Office 365, το Azure ή το Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1?ui=en-US&rs=en-US&ad=US)

[Επανειλημμένες ειδοποιήσεις για διαπιστευτήρια στο Office](https://docs.microsoft.com/office365/troubleshoot/authentication/access-denied-when-connect-to-office-365)