---
title: Αντιμετώπιση προβλημάτων σφαλμάτων στο OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 7fbc4617a0426eb11359339edc950a108f782750
ms.sourcegitcommit: 462522e6bccde76f6c46795b0eca71320c5d442d
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/15/2020
ms.locfileid: "44748919"
---
# <a name="troubleshoot-onedrive-crashes"></a>Αντιμετώπιση προβλημάτων σφαλμάτων στο OneDrive

Εάν το OneDrive διακοπεί επανειλημμένα, δοκιμάστε τα εξής βήματα αντιμετώπισης προβλημάτων:

**Βεβαιωθείτε ότι τα κλειδιά μητρώου δεν έχουν οριστεί:**

1. Χρήση του Επεξεργαστή Μητρώου( Registry Editor", μεταβείτε στην HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. Εάν υπάρχει το DisableFileSyncNGSC και οριστεί σε 1, ανοίξτε το κλειδί και αλλάξτε την τιμή σε 0.
3. Μη αυτόματη εκκίνηση του OneDrive μεταβαίνοντας στην Έναρξη ![Πάτημα του πλήκτρου των Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), πληκτρολογήστε OneDrive στο πλαίσιο αναζήτησης και, στη συνέχεια, κάντε κλικ στην εφαρμογή υπολογιστή OneDrive.

**Επαναφορά του OneDrive:**

Σημειώσεις:

- Η επαναφορά του OneDrive αποσυνδέει όλες τις υπάρχουσες συνδέσεις συγχρονισμού (συμπεριλαμβανομένου του προσωπικού σας OneDrive, αν έχει ρυθμιστεί).
- Δεν θα χάσετε αρχεία ή δεδομένα επαναφέροντας το OneDrive στον υπολογιστή σας.

**Για να επαναφέρετε το OneDrive:**

1. Ανοίξτε ένα παράθυρο διαλόγου Εκτέλεση πατώντας το πλήκτρο των Windows και το πλήκτρο R.
2. Πληκτρολογήστε %localappdata%\Microsoft\OneDrive\onedrive.exe /reset και πατήστε OK. Ένα παράθυρο εντολών μπορεί να εμφανιστεί για λίγο.
3. Μη αυτόματη εκκίνηση του OneDrive μεταβαίνοντας στην Έναρξη ![Πάτημα του πλήκτρου των Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), πληκτρολογήστε OneDrive στο πλαίσιο αναζήτησης και, στη συνέχεια, κάντε κλικ στην εφαρμογή υπολογιστή OneDrive.

Σημειώσεις:

- Εάν είχατε επιλέξει να συγχρονίσετε μόνο ορισμένους φακέλους πριν από την επαναφορά, θα πρέπει να το κάνετε ξανά μόλις ολοκληρωθεί ο συγχρονισμός. Διαβάστε την ενότητα [Επιλέξτε τους φακέλους του OneDrive που θα συγχρονιστούν με τον υπολογιστή σας](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)για   περισσότερες πληροφορίες.
- Θα χρειαστεί να το ολοκληρώσετε αυτό για το προσωπικό σας OneDrive και το OneDrive για επιχειρήσεις.