---
title: Ανάπτυξη εφαρμογών του Microsoft 365 για μεγάλες επιχειρήσεις για κοινόχρηστη χρήση σε RDS, Terminal Server ή VDI
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: a57be7fcf9d8236a51dc4b38e33ad1c2ac717f11
ms.sourcegitcommit: 2eab0980268e08a58014459d44a08a1cc34a17d4
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200673"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Ανάπτυξη εφαρμογών του Microsoft 365 για μεγάλες επιχειρήσεις για κοινόχρηστη χρήση σε RDS, Terminal Server ή VDI

Για να αναπτύξετε τις εφαρμογές Του Microsoft 365 για μεγάλες επιχειρήσεις χρησιμοποιώντας τις υπηρεσίες απομακρυσμένης επιφάνειας εργασίας (RDS), που ονομάζονταν παλαιότερα υπηρεσίες Terminal Services:

- Πρέπει να έχετε ένα πρόγραμμα του Microsoft 365 για επιχειρήσεις ή ένα πρόγραμμα του Office 365 που περιλαμβάνει τις Εφαρμογές Microsoft 365 για μεγάλες επιχειρήσεις, όπως το Office 365 για μεγάλες επιχειρήσεις E3 ή το E5 για μεγάλες επιχειρήσεις.
   > [!NOTE]
   > Τα προγράμματα Microsoft 365 Apps for business και Microsoft 365 Business Standard δεν περιλαμβάνουν τις Εφαρμογές Microsoft 365 για μεγάλες επιχειρήσεις.
- Πρέπει να ενεργοποιήσετε την [ενεργοποίηση κοινόχρηστου υπολογιστή.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

> [!NOTE]
> Μπορείτε επίσης να κάνετε λήψη και να εκτελέσετε τον Βοηθό υποστήριξης [και αποκατάστασης](https://aka.ms/SaRA_OfficeSCA_M365Portal) της Microsoft για να εγκαταστήσετε τις Εφαρμογές Microsoft 365 για μεγάλες επιχειρήσεις σε λειτουργία ενεργοποίησης κοινόχρηστου υπολογιστή.

Για περισσότερες πληροφορίες σχετικά με τα προαπαιτούμενα, τις οδηγίες ρύθμισης και τις οδηγίες σχετικά με τις προσαρμοσμένες εγκαταστάσεις χρησιμοποιώντας το Εργαλείο ανάπτυξης του Office, ανατρέξτε στο θέμα Ανάπτυξη εφαρμογών του Microsoft 365 για επιχειρήσεις με [χρήση των υπηρεσιών απομακρυσμένης επιφάνειας εργασίας.](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)

Για να διορθώσετε σφάλματα που σχετίζονται με την ενεργοποίηση κοινόχρηστου υπολογιστή:

- Ανατρέξτε [στο θέμα Αντιμετώπιση προβλημάτων με την ενεργοποίηση κοινόχρηστου υπολογιστή για εφαρμογές Microsoft 365 για μεγάλες επιχειρήσεις.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)
- Ανατρέξτε στο θέμα [Επαναφορά κατάστασης ενεργοποίησης των εφαρμογών Microsoft 365 για μεγάλες επιχειρήσεις](https://go.microsoft.com/fwlink/?linkid=2109218).

Εάν θέλετε να εγκαταστήσετε τις Εφαρμογές Microsoft 365 για μεγάλες επιχειρήσεις σε RDS από το Κέντρο διαχείρισης Microsoft 365, το οποίο χρησιμοποιεί προεπιλεγμένες ***ρυθμίσεις εγκατάστασης,*** ακολουθήστε τα παρακάτω βήματα:

1. Ελέγξτε ποια συνδρομή έχετε. [Μάθετε πώς](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2. Εάν είναι απαραίτητο, μεταβείτε σε διαφορετική συνδρομή. [Μάθετε πώς](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3. Εάν το Office είναι ήδη εγκατεστημένο στο διακομιστή RDS χρησιμοποιώντας οποιεσδήποτε άλλες συνδρομές της Microsoft, καταργήστε την εγκατάστασή του. Για παράδειγμα, εάν πρόκειται να καταργήσετε την **εγκατάσταση ενός** προγράμματος από τον  >  **Πίνακα Ελέγχου.** Καταργήστε την εγκατάσταση χρησιμοποιώντας τον Βοηθό υποστήριξης και αποκατάστασης της [Microsoft,](https://aka.ms/SARA-OfficeUninstall-Alchemy) εάν έχετε προβλήματα.
4. Στο διακομιστή RDS, πραγματοποιήστε είσοδο στο Κέντρο διαχείρισης Microsoft 365 με το λογαριασμό διαχειριστή σας και [εγκαταστήστε τις Εφαρμογές Microsoft 365 για μεγάλες επιχειρήσεις.](https://portal.office.com/OLS/MySoftware.aspx)
5. Μετά την εγκατάσταση του Office, ***μην ανοίξετε ή να εισέλθετε σε*** εφαρμογές του Office.
6. Στο διακομιστή RDS, ενεργοποιήστε την ενεργοποίηση κοινόχρηστου υπολογιστή, κάνοντας επεξεργασία του μητρώου, ακολουθώντας τα παρακάτω βήματα:
   1. Κάντε δεξί κλικ στο κουμπί των Windows στην κάτω αριστερή γωνία της οθόνης σας και επιλέξτε **"Εκτέλεση".** Στο πλαίσιο "Άνοιγμα", πληκτρολογήστε **regedit και,** στη συνέχεια, **επιλέξτε OK.**
   2. Επιλέξτε **"Ναι"** όταν σας ζητηθεί, για να επιτρέψετε στον Επεξεργαστή Μητρώου να κάνει αλλαγές στη συσκευή σας.
   3. Στον Επεξεργαστή Μητρώου, προσθέστε μια τιμή συμβολοσειράς **του SharedComputerLicensing** με ρύθμιση 1 στην περιοχή HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. Στο διακομιστή RDS,  πραγματοποιήστε είσοδο ως τελικός χρήστης και βεβαιωθείτε ότι η ενεργοποίηση κοινόχρηστου υπολογιστή είναι ενεργοποιημένη για τις εφαρμογές Microsoft [365 για μεγάλες επιχειρήσεις.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)
