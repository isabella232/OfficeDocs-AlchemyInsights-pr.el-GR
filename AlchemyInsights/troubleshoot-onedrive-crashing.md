---
title: Αντιμετώπιση προβλημάτων σφαλμάτων του OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 1155d370911b28bbb1ba83a15eace66d1daea28f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664998"
---
# <a name="troubleshoot-onedrive-crashes"></a>Αντιμετώπιση προβλημάτων σφαλμάτων του OneDrive

Εάν το OneDrive παρουσιάσει επανειλημμένα σφάλμα, δοκιμάστε αυτά τα βήματα αντιμετώπισης προβλημάτων:

**Βεβαιωθείτε ότι δεν έχουν καθοριστεί τα κλειδιά μητρώου:**

1. Χρησιμοποιώντας τον επεξεργαστή μητρώου, μεταβείτε στο HKEY_LOCAL_MACHINE \SOFTWARE\Policies\Microsoft\OneDrive
2. Εάν το DisableFileSyncNGSC είναι παρόν και ορίστε το 1, ανοίξτε το κλειδί και αλλάξτε την τιμή σε 0.
3. Μη αυτόματη εκκίνηση του OneDrive με τη μετάβαση στην έναρξη ![Πατήστε το πλήκτρο των Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), πληκτρολογήστε OneDrive στο πλαίσιο αναζήτησης και, στη συνέχεια, κάντε κλικ στην εφαρμογή υπολογιστή OneDrive.

**Επαναφορά του OneDrive:**

Σημειώσεις

- Η επαναφορά του OneDrive αποσυνδέει όλες τις υπάρχουσες συνδέσεις συγχρονισμού (συμπεριλαμβανομένου του προσωπικού σας OneDrive, εάν έχει ρυθμιστεί).
- Δεν θα χάσετε αρχεία ή δεδομένα με την επαναφορά του OneDrive στον υπολογιστή σας.

**Για να επαναφέρετε το OneDrive:**

1. Ανοίξτε ένα παράθυρο διαλόγου "εκτέλεση" πατώντας το πλήκτρο Windows και το πλήκτρο R.
2. Πληκτρολογήστε% localappdata% \Microsoft\OneDrive\onedrive.exe/reset και πατήστε OK. Ένα παράθυρο εντολών μπορεί να εμφανιστεί σύντομα.
3. Μη αυτόματη εκκίνηση του OneDrive με τη μετάβαση στην έναρξη ![Πατήστε το πλήκτρο των Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), πληκτρολογήστε OneDrive στο πλαίσιο αναζήτησης και, στη συνέχεια, κάντε κλικ στην εφαρμογή υπολογιστή OneDrive.

Σημειώσεις

- Εάν είχατε επιλέξει να συγχρονίσετε μόνο ορισμένους φακέλους πριν από την επαναφορά, θα πρέπει να το κάνετε ξανά όταν ολοκληρωθεί ο συγχρονισμός. Διαβάστε το στοιχείο [επιλογή των φακέλων του OneDrive για συγχρονισμό με τον υπολογιστή σας](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   για περισσότερες πληροφορίες.
- Θα πρέπει να το συμπληρώσετε αυτό για το προσωπικό σας OneDrive και το OneDrive για επιχείρηση.