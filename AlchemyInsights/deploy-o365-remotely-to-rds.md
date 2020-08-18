---
title: Ανάπτυξη εφαρμογών του Microsoft 365 για επιχειρήσεις για κοινή χρήση σε RDS, Terminal Server ή VDI
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: bd30d99221e3ddd0b07db0db78009f346babd2d0
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/17/2020
ms.locfileid: "46786277"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Ανάπτυξη εφαρμογών του Microsoft 365 για επιχειρήσεις για κοινή χρήση σε RDS, Terminal Server ή VDI

Για να αναπτύξετε τις εφαρμογές Microsoft 365 για επιχειρήσεις χρησιμοποιώντας τις υπηρεσίες απομακρυσμένης επιφάνειας εργασίας (RDS), οι οποίες παλαιότερα ονομάζονταν Terminal Services:
- Πρέπει να έχετε ένα πρόγραμμα του Microsoft 365 για επιχειρήσεις ή ένα πρόγραμμα του Office 365 που περιλαμβάνει εφαρμογές του Microsoft 365 για επιχειρήσεις, όπως το Office 365 Enterprise E3 ή το Enterprise E5.
   > [!NOTE] 
   > Τα προγράμματα Microsoft 365 apps για επιχειρήσεις και Microsoft 365 Business Premium Standard δεν περιλαμβάνουν εφαρμογές του Microsoft 365 για επιχειρήσεις.
- Πρέπει να ενεργοποιήσετε την [Ενεργοποίηση του κοινόχρηστου υπολογιστή](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

> [!NOTE]
> Μπορείτε επίσης να κάνετε λήψη και να εκτελέσετε τον [Βοηθό υποστήριξης και αποκατάστασης της Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) για να εγκαταστήσετε τις εφαρμογές Microsoft 365 για επιχειρήσεις σε λειτουργία ενεργοποίησης κοινόχρηστων υπολογιστών.

Για περισσότερες πληροφορίες σχετικά με τις προϋποθέσεις, τις οδηγίες εγκατάστασης και τις οδηγίες σχετικά με τις προσαρμοσμένες εγκαταστάσεις χρησιμοποιώντας το εργαλείο ανάπτυξης του Office, ανατρέξτε στο θέμα [ανάπτυξη εφαρμογών Microsoft 365 για επιχειρήσεις με τη χρήση υπηρεσιών απομακρυσμένης επιφάνειας εργασίας](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).

Για να διορθώσετε σφάλματα που σχετίζονται με την ενεργοποίηση του κοινόχρηστου υπολογιστή:
- Ανατρέξτε [στο θέμα Αντιμετώπιση προβλημάτων με την ενεργοποίηση του κοινόχρηστου υπολογιστή για εφαρμογές του Microsoft 365 για επιχειρήσεις](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
- Ανατρέξτε στο θέμα [Επαναφορά κατάστασης ενεργοποίησης των εφαρμογών Microsoft 365 για μεγάλες επιχειρήσεις](https://go.microsoft.com/fwlink/?linkid=2109218).

Εάν θέλετε να εγκαταστήσετε τις εφαρμογές του Microsoft 365 για επιχειρήσεις σε RDS από το κέντρο διαχείρισης του Microsoft 365, το ***οποίο χρησιμοποιεί τις προεπιλεγμένες ρυθμίσεις εγκατάστασης***, χρησιμοποιήστε τα παρακάτω βήματα:

1.    Επιλέξτε τη συνδρομή που έχετε. [Μάθετε πώς](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2.    Εάν είναι απαραίτητο, μεταβείτε σε διαφορετική συνδρομή. [Μάθετε πώς](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3.    Εάν το Office είναι ήδη εγκατεστημένο στο διακομιστή RDS χρησιμοποιώντας οποιεσδήποτε άλλες συνδρομές της Microsoft, καταργήστε την εγκατάστασή του. Για παράδειγμα, μεταβαίνοντας στον **πίνακα ελέγχου**,  >  **καταργήστε την εγκατάσταση ενός προγράμματος**. Καταργήστε την εγκατάσταση χρησιμοποιώντας [το βοηθό υποστήριξης και αποκατάστασης της Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) , εάν αντιμετωπίζετε προβλήματα.
4.    Στο διακομιστή RDS, πραγματοποιήστε είσοδο στο κέντρο διαχείρισης του Microsoft 365 με το λογαριασμό διαχειριστή σας και [Εγκαταστήστε τις εφαρμογές microsoft 365 για επιχειρήσεις](https://portal.office.com/OLS/MySoftware.aspx).
5.    Μετά την εγκατάσταση του Office, ***Μην ανοίγετε ή εισέρχεστε*** σε οποιαδήποτε εφαρμογή του Office.
6.    Στο διακομιστή RDS, ενεργοποιήστε την ενεργοποίηση του κοινόχρηστου υπολογιστή, επεξεργαζόμενοι το μητρώο ακολουθώντας τα παρακάτω βήματα:
   1. Κάντε δεξί κλικ στο κουμπί των Windows στην κάτω αριστερή γωνία της οθόνης σας και επιλέξτε **εκτέλεση**. Στο πλαίσιο Άνοιγμα, πληκτρολογήστε **regedit**και, στη συνέχεια, επιλέξτε **OK**.
   2. Επιλέξτε **Ναι** όταν σας ζητηθεί να επιτρέψετε στον επεξεργαστή μητρώου να κάνει αλλαγές στη συσκευή σας.
   3. Στον επεξεργαστή μητρώου, προσθέστε μια τιμή συμβολοσειράς του **SharedComputerLicensing** με μια ρύθμιση 1 στην περιοχή HKEY_LOCAL_MACHINE \software\microsoft \Office\ClickToRun\Configuration.
   4. Στο διακομιστή RDS, ***Πραγματοποιήστε είσοδο ως τελικός χρήστης*** και [Επαληθεύστε ότι η ενεργοποίηση του κοινόχρηστου υπολογιστή είναι ενεργοποιημένη για τις εφαρμογές Microsoft 365 για επιχειρήσεις](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

