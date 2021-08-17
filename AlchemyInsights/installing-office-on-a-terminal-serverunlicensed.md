---
title: Εγκατάσταση του office σε έναν Terminal Server - Χωρίς άδεια χρήσης
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 7e435df1515878ab4fe935ab8148daee29b8e3820095fc6e49db45de4c6279db
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54055158"
---
# <a name="installing-office-on-a-terminal-server"></a>Εγκατάσταση Office σε έναν Terminal Server

Για την ανάπτυξη Εφαρμογές Microsoft 365 για μεγάλες επιχειρήσεις σε έναν Windows χρησιμοποιώντας υπηρεσίες απομακρυσμένης επιφάνειας εργασίας (RDS), που ονομάζονταν παλαιότερα υπηρεσίες Terminal Services:
  
- Πρέπει να έχετε μια Microsoft 365 που περιλαμβάνει Εφαρμογές Microsoft 365 για μεγάλες επιχειρήσεις, όπως Office 365 για μεγάλες επιχειρήσεις E3 ή για μεγάλες επιχειρήσεις E5. Τα Εφαρμογές Microsoft 365 για επιχειρήσεις και Εφαρμογές Microsoft 365 για επιχειρήσεις Premium δεν περιλαμβάνουν Εφαρμογές Microsoft 365 για μεγάλες επιχειρήσεις.

- Πρέπει να ενεργοποιήσετε την [ενεργοποίηση κοινόχρηστου υπολογιστή.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

Εάν θέλετε να εγκαταστήσετε Εφαρμογές Microsoft 365 για μεγάλες επιχειρήσεις RDS από το Κέντρο διαχείρισης Microsoft 365, το οποίο χρησιμοποιεί προεπιλεγμένες ρυθμίσεις ***εγκατάστασης,*** ακολουθήστε τα παρακάτω βήματα.

> [!TIP]
> Μπορείτε επίσης να κάνετε λήψη και να εκτελέσετε το [Microsoft Βοηθός υποστήριξης και αποκατάστασης](https://aka.ms/SaRA_OfficeSCA_M365Portal) για να εγκαταστήσετε Εφαρμογές Microsoft 365 για μεγάλες επιχειρήσεις σε λειτουργία ενεργοποίησης κοινόχρηστου υπολογιστή.
  
1. Ελέγξτε τι Microsoft 365 συνδρομή που έχετε. [Μάθετε πώς](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. Εάν είναι απαραίτητο, μεταβείτε σε διαφορετική Microsoft 365 συνδρομής. [Μάθετε πώς](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Εάν Office ήδη εγκατεστημένο στο διακομιστή RDS χρησιμοποιώντας οποιεσδήποτε άλλες Microsoft 365 συνδρομές, καταργήστε την εγκατάστασή του. Για παράδειγμα, με την κατάργηση εγκατάστασης ενός προγράμματος από \> τον Πίνακα Ελέγχου. Καταργήστε [την εγκατάσταση χρησιμοποιώντας Βοηθός υποστήριξης και αποκατάστασης](https://aka.ms/SARA-OfficeUninstall-Alchemy) Microsoft, εάν έχετε προβλήματα.

4. Στο διακομιστή RDS, πραγματοποιήστε είσοδο στο Κέντρο διαχείρισης Microsoft 365 λογαριασμό διαχειριστή και [εγκαταστήστε το Εφαρμογές Microsoft 365 για μεγάλες επιχειρήσεις.](https://portal.office.com/OLS/MySoftware.aspx)

5. Αφού Office, μην ***ανοίγετε ή να*** μην εισέλθετε σε καμία Office εφαρμογών.

6. Στο διακομιστή RDS, ενεργοποιήστε την ενεργοποίηση κοινόχρηστου υπολογιστή, κάνοντας επεξεργασία του μητρώου, ακολουθώντας τα παρακάτω βήματα:

1. Κάντε δεξί κλικ στο Windows στην κάτω αριστερή γωνία της οθόνης σας και επιλέξτε "Εκτέλεση". Στο πλαίσιο "Άνοιγμα", πληκτρολογήστε **regedit και,** στη συνέχεια, επιλέξτε OK.

2. Επιλέξτε "Ναι" όταν σας ζητηθεί, για να επιτρέψετε στον Επεξεργαστή Μητρώου να κάνει αλλαγές στη συσκευή σας.

3. Στον Επεξεργαστή Μητρώου, προσθέστε μια τιμή συμβολοσειράς **του SharedComputerLicensing** με ρύθμιση 1 στην περιοχή HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. Στο διακομιστή RDS, ***πραγματοποιήστε είσοδο*** ως τελικός χρήστης και βεβαιωθείτε ότι η ενεργοποίηση κοινόχρηστου υπολογιστή [είναι ενεργοποιημένη για Εφαρμογές Microsoft 365 για μεγάλες επιχειρήσεις.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)

Για περισσότερες λεπτομέρειες σχετικά με τα προαπαιτούμενα, τις οδηγίες ρύθμισης και τις οδηγίες σχετικά με τις προσαρμοσμένες εγκαταστάσεις χρησιμοποιώντας το Εργαλείο ανάπτυξης Office, ανατρέξτε στο θέμα [Ανάπτυξη του Εφαρμογές Microsoft 365 για μεγάλες επιχειρήσεις χρησιμοποιώντας τις υπηρεσίες απομακρυσμένης επιφάνειας εργασίας.](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)
  
Για να διορθώσετε σφάλματα που σχετίζονται με την ενεργοποίηση κοινόχρηστου υπολογιστή, ανατρέξτε στο θέμα Αντιμετώπιση προβλημάτων με [την ενεργοποίηση κοινόχρηστου υπολογιστή για Εφαρμογές Microsoft 365 για μεγάλες επιχειρήσεις.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)
  