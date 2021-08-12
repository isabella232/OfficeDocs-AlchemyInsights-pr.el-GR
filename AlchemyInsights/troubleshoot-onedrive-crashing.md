---
title: Αντιμετώπιση προβλημάτων OneDrive σφαλμάτων
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
- "9003084"
- "5885"
ms.openlocfilehash: d5982bafbb8aaa1d240a34c071efe37e92c2ec5c5170dc59337df9a5435e22e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53921007"
---
# <a name="troubleshoot-onedrive-crashes"></a>Αντιμετώπιση προβλημάτων OneDrive σφαλμάτων

Εάν OneDrive επανειλημμένα σφάλμα, δοκιμάστε τα παρακάτω βήματα αντιμετώπισης προβλημάτων:

**Βεβαιωθείτε ότι δεν έχουν οριστεί κλειδιά μητρώου:**

1. Χρησιμοποιώντας τον Επεξεργαστή Μητρώου, μεταβείτε στην HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. Εάν το DisableFileSyncNGSC υπάρχει και έχει οριστεί σε 1, ανοίξτε το κλειδί και αλλάξτε την τιμή σε 0.
3. Εκκίνηση με μη αυτόματο OneDrive από την Έναρξη ![Πατήστε το Windows πλήκτρο](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), πληκτρολογήστε OneDrive στο πλαίσιο αναζήτησης και, στη συνέχεια, κάντε κλικ στην OneDrive υπολογιστή.

**Επαναφορά OneDrive:**

Σημειώσεις:

- Η επαναφορά OneDrive αποσυνδέει όλες τις υπάρχουσες συνδέσεις συγχρονισμού (συμπεριλαμβανομένων των προσωπικών OneDrive εάν έχει ρυθμιστεί).
- Δεν θα χάσετε αρχεία ή δεδομένα κάνοντας επαναφορά OneDrive υπολογιστή σας.

**Για να επαναφέρετε OneDrive:**

1. Ανοίξτε ένα παράθυρο διαλόγου "Εκτέλεση" πατώντας Windows και R.
2. Πληκτρολογήστε %localappdata%\Microsoft\OneDrive\onedrive.exe /reset και πατήστε το πλήκτρο OK. Ένα παράθυρο εντολών μπορεί να εμφανιστεί για λίγο.
3. Εκκίνηση με μη αυτόματο OneDrive από την Έναρξη ![Πατήστε το Windows πλήκτρο](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), πληκτρολογήστε OneDrive στο πλαίσιο αναζήτησης και, στη συνέχεια, κάντε κλικ στην OneDrive υπολογιστή.

Σημειώσεις:

- Εάν είχατε επιλέξει να συγχρονίσετε μόνο ορισμένους φακέλους πριν από την επαναφορά, θα πρέπει να το κάνετε ξανά μόλις ολοκληρωθεί ο συγχρονισμός. Διαβάστε [την επιλογή OneDrive φακέλων που θα συγχρονίζονται με τον υπολογιστή](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)σας για περισσότερες   πληροφορίες.
- Θα πρέπει να το ολοκληρώσετε αυτό για τις προσωπικές σας OneDrive και OneDrive για επιχειρήσεις.