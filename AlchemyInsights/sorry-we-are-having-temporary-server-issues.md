---
title: Επιδιόρθωση εφαρμογών Microsoft 365 Λυπούμαστε, αντιμετωπίζουμε ένα προσωρινό μήνυμα προβλημάτων διακομιστή
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
- "3420"
- "9001430"
ms.openlocfilehash: 565f70d9a09c61bef84cdd1c23e9b0ed34bebe51
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744646"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Επιδιόρθωση του μηνύματος Microsoft 365 εφαρμογών "Λυπούμαστε, αντιμετωπίζουμε προσωρινά προβλήματα διακομιστή"

Σημείωση: Εάν χρησιμοποιείτε μια παλαιότερη έκδοση του Windows (π.χ. Windows 7 SP1, Windows Server 2008 R2), χρησιμοποιήστε την [εύκολη επιδιόρθωση](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) για να ενεργοποιήσετε το TLS 1.2 ως προεπιλογή. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Ενημέρωση για την ενεργοποίηση των TLS 1.1 και TLS 1.2 ως προεπιλεγμένων ασφαλών πρωτοκόλλων στο WinHTTP στο Windows.](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Εάν λάβετε αυτό το μήνυμα, δοκιμάστε τα εξής:

1. Ελέγξτε τις ρυθμίσεις τείχους προστασίας, λογισμικού προστασίας από ιούς και διακομιστή μεσολάβησης για να επιβεβαιώσετε ότι δεν αποκλείουν την πρόσβαση στο Internet για να Microsoft 365 εφαρμογές. Ανατρέξτε στο θέμα [Διευθύνσεις URL και περιοχές διευθύνσεων IP.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Μεταβείτε στην **Έναρξη**  >  **Εκτέλεση** και, στη συνέχεια, πληκτρολογήστε **services.msc**. Βεβαιωθείτε ότι όλες οι ακόλουθες υπηρεσίες εκτελούνται:
    - Αυτόματη εγκατάσταση συνδεδεμένων συσκευών δικτύου
    - Υπηρεσία λίστας δικτύου
    - Αναγνώριση θέσης δικτύου
    - Windows Αρχείο καταγραφής συμβάντων

Εάν μία από αυτές τις υπηρεσίες δεν εκτελείται, προσπαθήστε να την εκκινήσετε. Εάν αντιμετωπίζετε πρόβλημα κατά την εκκίνηση της υπηρεσίας, εκτελέστε την ακόλουθη εντολή ανοίγοντας μια γραμμή εντολών με αναβαθμισμένες άδειες:

**sfc /scannow**

Μετά την ολοκλήρωση αυτής της εντολής, επανεκκινήστε τον υπολογιστή.

Για λεπτομερείς πληροφορίες, ανατρέξτε στο θέμα ["Λυπούμαστε, δεν μπορούμε να συνδεθούμε στο λογαριασμό σας. Δοκιμάστε ξανά αργότερα" κατά την ενεργοποίηση](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)του .