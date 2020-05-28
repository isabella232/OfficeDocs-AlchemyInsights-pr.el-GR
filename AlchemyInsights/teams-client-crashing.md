---
title: Σφάλματα στο πρόγραμμα-πελάτη Teams;
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ac1cc05adfa33626ff34d30dca6c77f1bb96477a
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 05/23/2020
ms.locfileid: "44354052"
---
# <a name="teams-client-crashing"></a>Σφάλματα στο πρόγραμμα-πελάτη Teams;

Εάν το πρόγραμμα-πελάτης του Teams σας παρουσιάζει σφάλματα, δοκιμάστε τα εξής:

- Εάν χρησιμοποιείτε την εφαρμογή υπολογιστή Teams, [βεβαιωθείτε ότι η εφαρμογή είναι πλήρως ενημερωμένη](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Βεβαιωθείτε ότι είναι προσβάσιμες όλες οι [διευθύνσεις URL και οι περιοχές διευθύνσεων του Microsoft 365.](https://docs.microsoft.com/microsoftteams/connectivity-issues)

- Συνδεθείτε με το λογαριασμό διαχειριστή μισθωτή και ελέγξτε [τον πίνακα εργαλείων εύρυθμης λειτουργίας υπηρεσίας](https://docs.microsoft.com/office365/enterprise/view-service-health) για να βεβαιωθείτε ότι δεν υπάρχει διακοπή ρεύματος ή υποβάθμιση της υπηρεσίας.

- Κατάργηση εγκατάστασης και επανεγκατάσταση της εφαρμογής teams (link)
    - Μεταβείτε στο φάκελο %appdata%\Microsoft\teams\ στον υπολογιστή σας και διαγράψτε όλα τα αρχεία σε αυτόν τον κατάλογο.
    - [Κατεβάστε και εγκαταστήστε την εφαρμογή Teams](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)και, εάν είναι δυνατόν, εγκαταστήστε το Teams ως διαχειριστή (κάντε δεξί κλικ στο πρόγραμμα εγκατάστασης ομάδων και επιλέξτε "Εκτέλεση ως διαχειριστής" εάν είναι διαθέσιμο).

Εάν το πρόγραμμα-πελάτης του Teams εξακολουθεί να είναι σε αιφνίδια διακοπή λειτουργίας, μπορείτε να αναπαραγάγετε το ζήτημα; Αν ναι:

1. Χρησιμοποιήστε την Καταγραφή βημάτων για να καταγράψετε τα βήματά σας.
    - Κλείστε όλες τις περιττές ή εμπιστευτικές εφαρμογές.
    - Εκκινήστε την Καταγραφή βημάτων και αναπαράγνατε το ζήτημα ενώ είστε συνδεδεμένοι με το λογαριασμό χρήστη που επηρεάζεται.
    - [Συλλέξτε τα αρχεία καταγραφής ομάδων που αποτυπώνουν τα καταγεγραμμένα βήματα αναπαραγωγής](https://docs.microsoft.com/microsoftteams/log-files). **Σημείωση**: Βεβαιωθείτε ότι καταγράφετε τη διεύθυνση εισόδου του χρήστη που επηρεάζεται.
    - Συλλέξτε τις πληροφορίες κάδο χωματερή ς ή/και βλαβών (Windows). Εκκίνηση του Windows Powershell στον υπολογιστή όπου παρουσιάζεται η αιφνίδια διακοπή λειτουργίας και εκτελέστε τις ακόλουθες εντολές:

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. Επισυνάψτε το αρχείο στην υπόθεση υποστήριξης.
