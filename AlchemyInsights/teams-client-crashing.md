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
ms.openlocfilehash: ce37b260d126f876d2b6177515bd8a7c3874ef2c
ms.sourcegitcommit: d02e2b73aa7d0453d7baca1ea5a186cf6081d022
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 03/27/2020
ms.locfileid: "43030583"
---
# <a name="teams-client-crashing"></a>Σφάλματα στο πρόγραμμα-πελάτη Teams;

Εάν το πρόγραμμα-πελάτης του Teams σας παρουσιάζει σφάλματα, δοκιμάστε τα εξής:

- Εάν χρησιμοποιείτε την εφαρμογή υπολογιστή Teams, [βεβαιωθείτε ότι η εφαρμογή είναι πλήρως ενημερωμένη](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Βεβαιωθείτε ότι έχετε πρόσβαση σε όλες τις [περιοχές διευθύνσεων URL και διευθύνσεις του Office 365](https://docs.microsoft.com/microsoftteams/connectivity-issues).

- Συνδεθείτε με τον λογαριασμό διαχειριστή σας και ελέγξτε τον [Πίνακα ελέγχου εύρυθμης λειτουργίας υπηρεσιών](https://docs.microsoft.com/office365/enterprise/view-service-health) για να επαληθεύσετε ότι δεν υπάρχει διακοπή λειτουργίας ή υποβάθμιση υπηρεσίας.

 - Ως τελευταίο βήμα, μπορείτε να επιχειρήσετε την εκκαθάριση της μνήμης cache του προγράμματος-πελάτη Teams:

    1.  Τερματίστε πλήρως το πρόγραμμα-πελάτη υπολογιστή Microsoft Teams. Μπορείτε να κάνετε δεξί κλικ στο **Teams** από τον δίσκο εικονιδίων και να κάνετε κλικ στην επιλογή **Κλείσιμο** ή να εκτελέσετε τη Διαχείριση εργασιών και να σταματήσετε πλήρως τη διαδικασία.

    2.  Μεταβείτε στην Εξερεύνηση αρχείων και πληκτρολογήστε "%appdata%\Microsoft\teams".

    3.  Αφού βρεθείτε στον κατάλογο, θα δείτε μερικούς από τους ακόλουθους φακέλους:

         - Μέσα από το **Μνήμη cache εφαρμογών**, μεταβείτε στη Μνήμη cache και διαγράψτε οποιοδήποτε από τα αρχεία στη θέση cache: %appdata%\Microsoft\teams\application cache\cache.

        - Μέσα από το **Blob_storage**, διαγράψτε όλα τα αρχεία: %appdata%\Microsoft\teams\blob_storage.

        - Μέσα από τη **Μνήμη cache**, διαγράψτε όλα τα αρχεία: %appdata%\Microsoft\teams\Cache.

        - Μέσα από τις **βάσεις δεδομένων**, διαγράψτε όλα τα αρχεία: %appdata%\Microsoft\teams\databases.

        - Μέσα από τη **Μνήμη GPUcache**, διαγράψτε όλα τα αρχεία: %appdata%\Microsoft\teams\GPUcache.

        - Μέσα από το **IndexedDB**, διαγράψτε το αρχείο .db: %appdata%\Microsoft\teams\IndexedDB.

        - Μέσα από τον **Τοπικό χώρο αποθήκευσης**, διαγράψτε όλα τα αρχεία: %appdata%\Microsoft\teams\Local Storage.

        - Τέλος, μέσα από το **tmp**, διαγράψτε οποιοδήποτε αρχείο: %appdata%\Microsoft\teams\tmp.

    4. Επανεκκινήστε το πρόγραμμα-πελάτη Teams.
