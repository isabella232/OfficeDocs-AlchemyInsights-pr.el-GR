---
title: Teams προγράμματος-πελάτη παρουσιάζει σφάλμα
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
ms.openlocfilehash: bef16351b55ac4765539d66ab86a71183f66f0dd
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321625"
---
# <a name="teams-client-crashing"></a>Teams προγράμματος-πελάτη παρουσιάζει σφάλμα

Εάν το πρόγραμμα-πελάτης του Teams σας παρουσιάζει σφάλματα, δοκιμάστε τα εξής:

- Εάν χρησιμοποιείτε την εφαρμογή υπολογιστή Teams, [βεβαιωθείτε ότι η εφαρμογή είναι πλήρως ενημερωμένη](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Βεβαιωθείτε ότι όλες οι Microsoft 365 διευθύνσεων URL [και οι περιοχές διευθύνσεων](https://docs.microsoft.com/microsoftteams/connectivity-issues) είναι προσβάσιμες.

- Συνδεθείτε με το λογαριασμό διαχειριστή μισθωτή και ελέγξτε τον πίνακα εργαλείων της υπηρεσίας [υγείας](https://docs.microsoft.com/office365/enterprise/view-service-health) για να βεβαιωθείτε ότι δεν υπάρχει καμία υποβάθμιση της υπηρεσίας.

- Κατάργηση εγκατάστασης και επανεγκατάσταση της Teams εφαρμογής
    - Μεταβείτε στο φάκελο %appdata%\Microsoft\Teams\ στον υπολογιστή σας και διαγράψτε όλα τα αρχεία σε αυτόν τον κατάλογο.
    - [Κάντε λήψη και εγκατάσταση της εφαρμογής Teams και,](https://www.microsoft.com/microsoft-teams/download-app)εάν είναι δυνατό, εγκαταστήστε το Teams ως διαχειριστής (κάντε δεξί κλικ στο πρόγραμμα εγκατάστασης του Teams και επιλέξτε "Εκτέλεση ως **διαχειριστής",** εάν είναι διαθέσιμο).

Εάν το πρόγραμμα Teams εξακολουθεί να παρουσιάζει σφάλμα, προσπαθήστε να αναπαραγάγετε το πρόβλημα. Εάν μπορείτε να κάνετε τα εξής:

1. Χρησιμοποιήστε την Καταγραφή βημάτων για να καταγράψετε τα βήματά σας.
    - Κλείστε ΌΛΕς τις περιττές ή εμπιστευτικές εφαρμογές.
    - Εκκινηθείτε την Καταγραφή βημάτων και αναπαραγάγετε το πρόβλημα ενώ είστε συνδεδεμένοι με το λογαριασμό χρήστη που επηρεάζεται.
    - [Συλλέξτε τα αρχεία καταγραφής ομάδων που καταγραφούν τα βήματα της καταγεγραμμένης διαδικασίας repro.](https://docs.microsoft.com/microsoftteams/log-files) 
    
    **Σημείωση:** Βεβαιωθείτε ότι καταγράψετε τη διεύθυνση της είσοδος του χρήστη που έχει επιπτώσεις.
    - Συλλέξτε πληροφορίες κάδου απόρριψης ή/και σφάλματος (Windows). Ξεκινήστε Windows Powershell στον υπολογιστή όπου παρουσιάζεται το σφάλμα και εκτελέστε τις ακόλουθες εντολές (μετά από κάθε εντολή, πατήστε το πλήκτρο Enter):

    `cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`
    `notepad .\FaultBuckets.txt`
    
2. Αφού δημιουργηθεί το αρχείο κειμένου και εμφανιστεί στην οθόνη σας, αποθηκεύστε το αρχείο και επισυνάψτε το στην αίτηση υπηρεσίας. 
