---
title: Εγκατάσταση γραφείου σε terminal server - Χωρίς άδεια χρήσης
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 6e952513679c9ac66f8de2b43d6d243cf17ff789
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010614"
---
# <a name="installing-office-on-a-terminal-server"></a>Εγκατάσταση του Office σε διακομιστή τερματικού

Για την ανάπτυξη εφαρμογών microsoft 365 για επιχειρήσεις σε διακομιστή των Windows χρησιμοποιώντας τις υπηρεσίες απομακρυσμένης επιφάνειας εργασίας (RDS), οι υπηρεσίες Terminal Services που παλαιότερα ονομάζονταν:10
  
- Πρέπει να έχετε μια συνδρομή Microsoft 365 που περιλαμβάνει εφαρμογές της Microsoft 365 για μεγάλες επιχειρήσεις, όπως το Office 365 για μεγάλες επιχειρήσεις E3 ή για μεγάλες επιχειρήσεις E5. Οι εφαρμογές microsoft 365 για επιχειρήσεις και οι εφαρμογές Microsoft 365 για προγράμματα Premium για επιχειρήσεις δεν περιλαμβάνουν εφαρμογές της Microsoft 365 για επιχειρήσεις.

- Πρέπει να ενεργοποιήσετε την [ενεργοποίηση κοινόχρηστου υπολογιστή](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

Εάν θέλετε να εγκαταστήσετε τις Εφαρμογές Microsoft 365 για μεγάλες επιχειρήσεις σε RDS από το κέντρο διαχείρισης του Microsoft 365, ***το οποίο χρησιμοποιεί προεπιλεγμένες ρυθμίσεις εγκατάστασης***, χρησιμοποιήστε τα ακόλουθα βήματα.

> [!TIP]
> Μπορείτε επίσης να κάνετε λήψη και εκτέλεση του [Βοηθού υποστήριξης και αποκατάστασης της Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) για να εγκαταστήσετε τις Εφαρμογές Microsoft 365 για επιχειρήσεις σε κατάσταση ενεργοποίησης κοινόχρηστου υπολογιστή.
  
1. Ελέγξτε τι συνδρομή microsoft 365 που έχετε. [Μάθετε πώς](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. Εάν είναι απαραίτητο, μεταβείτε σε διαφορετική συνδρομή Microsoft 365. [Μάθετε πώς](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. Εάν το Office είναι ήδη εγκατεστημένο στο διακομιστή RDS χρησιμοποιώντας οποιεσδήποτε άλλες συνδρομές του Microsoft 365, καταργήστε την εγκατάστασή του. Για παράδειγμα, μεταβαίνωσε στον Πίνακα \> Ελέγχου Κατάργηση εγκατάστασης ενός προγράμματος. Καταργήστε την εγκατάσταση [χρησιμοποιώντας το Βοηθό υποστήριξης και αποκατάστασης της Microsoft,](https://aka.ms/SARA-OfficeUninstall-Alchemy) εάν εξαντλείστε προβλήματα.

4. Στο διακομιστή RDS, συνδεθείτε στο κέντρο διαχείρισης του Microsoft 365 με το λογαριασμό διαχειριστή και [εγκαταστήστε τις Εφαρμογές Microsoft 365 για μεγάλες επιχειρήσεις](https://portal.office.com/OLS/MySoftware.aspx).

5. Μετά την εγκατάσταση του Office, ***μην ανοίξετε ή εισέλθετε σε*** εφαρμογές του Office.

6. Στο διακομιστή RDS, ενεργοποιήστε την ενεργοποίηση κοινόχρηστου υπολογιστή με επεξεργασία του μητρώου, ακολουθώντας τα εξής βήματα:

1. Κάντε δεξί κλικ στο κουμπί των Windows στην κάτω αριστερή γωνία της οθόνης σας και επιλέξτε Εκτέλεση. Στο πλαίσιο Άνοιγμα, πληκτρολογήστε **regedit**και, στη συνέχεια, επιλέξτε OK.

2. Επιλέξτε Ναι όταν σας ζητηθεί να επιτρέψετε στον Επεξεργαστή Μητρώου (Registry Editor) να κάνει αλλαγές στη συσκευή σας.

3. Στον Επεξεργαστή Μητρώου (Registry Editor), προσθέστε μια τιμή συμβολοσειράς της **άδειας χρήσης κοινόχρηστου υπολογιστή** με ρύθμιση 1 υπό HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. Στο διακομιστή RDS, ***εισέλθετε ως τελικός χρήστης*** και [βεβαιωθείτε ότι είναι ενεργοποιημένη η ενεργοποίηση κοινόχρηστου υπολογιστή για εφαρμογές Microsoft 365 για επιχειρήσεις](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

Για περισσότερες λεπτομέρειες σχετικά με τις προϋποθέσεις, τις οδηγίες εγκατάστασης και τις οδηγίες σχετικά με τις προσαρμοσμένες εγκαταστάσεις χρησιμοποιώντας το Εργαλείο ανάπτυξης του Office, ανατρέξτε στο θέμα [Ανάπτυξη εφαρμογών του Microsoft 365 για επιχειρήσεις χρησιμοποιώντας τις υπηρεσίες απομακρυσμένης επιφάνειας εργασίας](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).
  
Για να διορθώσετε σφάλματα που σχετίζονται με την ενεργοποίηση κοινόχρηστου υπολογιστή, ανατρέξτε στο θέμα [Αντιμετώπιση προβλημάτων με την ενεργοποίηση κοινόχρηστου υπολογιστή για εφαρμογές microsoft 365 για επιχειρήσεις](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
  