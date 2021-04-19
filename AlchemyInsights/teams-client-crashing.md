---
title: Σφάλματα στο πρόγραμμα-πελάτη Teams;
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: 20f03b075787cab85ab15d5272c0416b88ebbaee
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826271"
---
# <a name="teams-client-crashing"></a>Σφάλματα στο πρόγραμμα-πελάτη Teams;

Εάν το πρόγραμμα-πελάτης του Teams σας παρουσιάζει σφάλματα, δοκιμάστε τα εξής:

- Εάν χρησιμοποιείτε την εφαρμογή υπολογιστή Teams, [βεβαιωθείτε ότι η εφαρμογή είναι πλήρως ενημερωμένη](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Βεβαιωθείτε ότι όλες οι διευθύνσεις URL και οι περιοχές διευθύνσεων του [Microsoft 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) είναι προσβάσιμες.

- Συνδεθείτε με το λογαριασμό διαχειριστή μισθωτή και ελέγξτε τον πίνακα εργαλείων της υπηρεσίας [υγείας](https://docs.microsoft.com/office365/enterprise/view-service-health) για να βεβαιωθείτε ότι δεν υπάρχει καμία υποβάθμιση της υπηρεσίας.

- Κατάργηση εγκατάστασης και επανεγκατάσταση της εφαρμογής Teams (σύνδεση)
    - Μεταβείτε στο φάκελο %appdata%\Microsoft\teams\ στον υπολογιστή σας και διαγράψτε όλα τα αρχεία σε αυτόν τον κατάλογο.
    - [Κάντε λήψη και εγκατάσταση της εφαρμογής Teams](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)και, εάν είναι δυνατό, εγκαταστήστε το Teams ως διαχειριστή (κάντε δεξί κλικ στο πρόγραμμα εγκατάστασης του Teams και επιλέξτε "Εκτέλεση ως διαχειριστής", εάν είναι διαθέσιμο).

Εάν το πρόγραμμα-πελάτης του Teams εξακολουθεί να παρουσιάζει σφάλμα, μπορείτε να αναπαραγάγετε το πρόβλημα; Εάν ναι:

1. Χρησιμοποιήστε την Καταγραφή βημάτων για να καταγράψετε τα βήματά σας.
    - Κλείστε ΌΛΕς τις περιττές ή εμπιστευτικές εφαρμογές.
    - Εκκινηθείτε την Καταγραφή βημάτων και αναπαραγάγετε το πρόβλημα ενώ είστε συνδεδεμένοι με το λογαριασμό χρήστη που επηρεάζεται.
    - [Συλλέξτε τα αρχεία καταγραφής ομάδων που καταγραφούν τα βήματα της καταγεγραμμένης διαδικασίας repro.](https://docs.microsoft.com/microsoftteams/log-files) **Σημείωση:** Βεβαιωθείτε ότι καταγράψετε τη διεύθυνση της είσοδος του χρήστη που έχει επιπτώσεις.
    - Συλλέξτε πληροφορίες κάδου απόρριψης ή/και σφάλματος (Windows). Εκκινήστε το Windows Powershell στον υπολογιστή όπου παρουσιάζεται το σφάλμα και εκτελέστε τις ακόλουθες εντολές:

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. Επισυνάψτε το αρχείο στην υπόθεση υποστήριξης.
