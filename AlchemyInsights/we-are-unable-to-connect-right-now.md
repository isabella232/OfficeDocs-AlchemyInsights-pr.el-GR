---
title: Πρόβλημα ενεργοποίησης - Δεν είναι δυνατή η σύνδεση αυτήν τη στιγμή
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
- "3408"
- "9001423"
ms.openlocfilehash: 0ab831696736352bf9de84f43c96bb8f7238d8eb
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744595"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Επιδιόρθωση του μηνύματος Microsoft 365 εφαρμογών "Δεν είναι δυνατή η σύνδεση αυτήν τη στιγμή"

Σημείωση: Εάν χρησιμοποιείτε μια παλαιότερη έκδοση του Windows (π.χ. Windows 7 SP1, Windows Server 2008 R2), χρησιμοποιήστε την [εύκολη επιδιόρθωση](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) για να ενεργοποιήσετε το TLS 1.2 ως προεπιλογή. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα Ενημέρωση για την ενεργοποίηση των [TLS 1.1 και TLS 1.2 ως προεπιλεγμένων ασφαλών πρωτοκόλλων στο WinHTTP στο Windows.](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Εάν λάβετε αυτό το μήνυμα, δοκιμάστε τα εξής:

1. Ελέγξτε το τείχος προστασίας, το λογισμικό προστασίας από ιούς και τις ρυθμίσεις του διακομιστή μεσολάβησης για να επιβεβαιώσετε ότι δεν αποκλείουν την πρόσβαση στο Internet για να Microsoft 365 εφαρμογές. Ανατρέξτε στο θέμα [Διευθύνσεις URL και περιοχές διευθύνσεων IP της Microsoft.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Μεταβείτε στην **Έναρξη**  >  **Εκτέλεση** και, στη συνέχεια, πληκτρολογήστε **services.msc**. Βεβαιωθείτε ότι όλες οι ακόλουθες υπηρεσίες εκτελούνται:
    - Αυτόματη εγκατάσταση συνδεδεμένων συσκευών δικτύου
    - Υπηρεσία λίστας δικτύου
    - Αναγνώριση θέσης δικτύου
    - Windows Αρχείο καταγραφής συμβάντων

Εάν μία από αυτές τις υπηρεσίες δεν εκτελείται, προσπαθήστε να την εκκινήσετε. Εάν αντιμετωπίζετε πρόβλημα κατά την εκκίνηση της υπηρεσίας, εκτελέστε την ακόλουθη εντολή ανοίγοντας μια γραμμή εντολών με αναβαθμισμένες άδειες:

**sfc /scannow**

Μετά την ολοκλήρωση αυτής της εντολής, επανεκκινήστε τον υπολογιστή.

Για λεπτομερείς πληροφορίες, ανατρέξτε στο θέμα ["Λυπούμαστε, δεν μπορούμε να συνδεθούμε στο λογαριασμό σας. Δοκιμάστε ξανά αργότερα", κατά την ενεργοποίηση Office από το Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).