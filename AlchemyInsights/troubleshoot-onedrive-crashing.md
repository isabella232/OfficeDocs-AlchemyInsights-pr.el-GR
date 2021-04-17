---
title: Αντιμετώπιση προβλημάτων σφαλμάτων του OneDrive
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
ms.openlocfilehash: 4bf45e7780dcbabb95b3eecfb2df55beffde11d6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826199"
---
# <a name="troubleshoot-onedrive-crashes"></a>Αντιμετώπιση προβλημάτων σφαλμάτων του OneDrive

Εάν το OneDrive παρουσιάζει επανειλημμένα σφάλμα, δοκιμάστε τα παρακάτω βήματα αντιμετώπισης προβλημάτων:

**Βεβαιωθείτε ότι δεν έχουν οριστεί κλειδιά μητρώου:**

1. Χρησιμοποιώντας τον Επεξεργαστή Μητρώου, μεταβείτε στην HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. Εάν το DisableFileSyncNGSC υπάρχει και έχει οριστεί σε 1, ανοίξτε το κλειδί και αλλάξτε την τιμή σε 0.
3. Εκκίνηση του OneDrive με μη αυτόματο τρόπο, στην Έναρξη ![Πατήστε το πλήκτρο των Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), πληκτρολογήστε το OneDrive στο πλαίσιο αναζήτησης και, στη συνέχεια, κάντε κλικ στην εφαρμογή υπολογιστή OneDrive.

**Επαναφορά του OneDrive:**

Σημειώσεις:

- Η επαναφορά του OneDrive αποσυνδέει όλες τις υπάρχουσες συνδέσεις συγχρονισμού (συμπεριλαμβανομένου του προσωπικού σας OneDrive, εάν έχει ρυθμιστεί).
- Δεν θα χάσετε αρχεία ή δεδομένα με την επαναφορά του OneDrive στον υπολογιστή σας.

**Για να επαναφέρετε το OneDrive:**

1. Ανοίξτε ένα παράθυρο διαλόγου "Εκτέλεση" πατώντας το πλήκτρο των Windows και το πλήκτρο R.
2. Πληκτρολογήστε %localappdata%\Microsoft\OneDrive\onedrive.exe /reset και πατήστε το πλήκτρο OK. Ένα παράθυρο εντολών μπορεί να εμφανιστεί για λίγο.
3. Εκκίνηση του OneDrive με μη αυτόματο τρόπο, στην Έναρξη ![Πατήστε το πλήκτρο των Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), πληκτρολογήστε το OneDrive στο πλαίσιο αναζήτησης και, στη συνέχεια, κάντε κλικ στην εφαρμογή υπολογιστή OneDrive.

Σημειώσεις:

- Εάν είχατε επιλέξει να συγχρονίσετε μόνο ορισμένους φακέλους πριν από την επαναφορά, θα πρέπει να το κάνετε ξανά μόλις ολοκληρωθεί ο συγχρονισμός. Διαβάστε [την επιλογή των φακέλων του OneDrive που θα συγχρονιστούν με τον υπολογιστή](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)σας για περισσότερες   πληροφορίες.
- Θα πρέπει να το ολοκληρώσετε αυτό για το προσωπικό σας OneDrive και το OneDrive για επιχειρήσεις.