---
title: Ανάπτυξη εφαρμογών της Microsoft 365 για επιχειρήσεις για κοινή χρήση σε RDS, Terminal Server ή VDI
ms.author: v-todmc
author: todmccoy
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
ms.openlocfilehash: fe051cd1dac899dc9bb19d275c352ec6585b6a93
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507586"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Ανάπτυξη εφαρμογών της Microsoft 365 για επιχειρήσεις για κοινή χρήση σε RDS, Terminal Server ή VDI

Για να αναπτύξετε εφαρμογές της Microsoft 365 για επιχειρήσεις χρησιμοποιώντας τις υπηρεσίες απομακρυσμένης επιφάνειας εργασίας (RDS), οι υπηρεσίες Terminal Services που παλαιότερα ονομάζονταν:10
- Πρέπει να έχετε ένα πρόγραμμα microsoft 365 για επιχειρήσεις ή ένα πρόγραμμα του Office 365 που περιλαμβάνει εφαρμογές της Microsoft 365 για μεγάλες επιχειρήσεις, όπως το Office 365 για μεγάλες επιχειρήσεις E3 ή το Enterprise E5.
   > [!NOTE] 
   > Τα προγράμματα Microsoft 365 Apps για επιχειρήσεις και Microsoft 365 Premium Premium για επιχειρήσεις δεν περιλαμβάνουν εφαρμογές της Microsoft 365 για επιχειρήσεις.
- Πρέπει να ενεργοποιήσετε [την ενεργοποίηση κοινόχρηστου υπολογιστή](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

> [!NOTE]
> Μπορείτε επίσης να κάνετε λήψη και εκτέλεση του [Βοηθού υποστήριξης και αποκατάστασης της Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) για να εγκαταστήσετε τις Εφαρμογές Microsoft 365 για επιχειρήσεις σε κατάσταση ενεργοποίησης κοινόχρηστου υπολογιστή.

Για περισσότερες πληροφορίες σχετικά με τις προϋποθέσεις, τις οδηγίες εγκατάστασης και τις οδηγίες σχετικά με τις προσαρμοσμένες εγκαταστάσεις χρησιμοποιώντας το Εργαλείο ανάπτυξης του Office, ανατρέξτε στο θέμα [Ανάπτυξη εφαρμογών του Microsoft 365 για επιχειρήσεις χρησιμοποιώντας τις υπηρεσίες απομακρυσμένης επιφάνειας εργασίας](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).

Για να διορθώσετε σφάλματα που σχετίζονται με την ενεργοποίηση κοινόχρηστου υπολογιστή:
- Ανατρέξτε [στο θέμα Αντιμετώπιση προβλημάτων με την ενεργοποίηση κοινόχρηστου υπολογιστή για εφαρμογές microsoft 365 για επιχειρήσεις](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
- Ανατρέξτε στο θέμα [Επαναφορά κατάστασης ενεργοποίησης των εφαρμογών Microsoft 365 για μεγάλες επιχειρήσεις](https://go.microsoft.com/fwlink/?linkid=2109218).

Εάν θέλετε να εγκαταστήσετε τις Εφαρμογές Microsoft 365 για μεγάλες επιχειρήσεις σε RDS από το κέντρο διαχείρισης του Microsoft 365, ***το οποίο χρησιμοποιεί προεπιλεγμένες ρυθμίσεις εγκατάστασης***, ακολουθήστε τα ακόλουθα βήματα:

1.    Ελέγξτε τι συνδρομή έχετε. [Μάθετε πώς](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2.    Εάν είναι απαραίτητο, μεταβείτε σε διαφορετική συνδρομή. [Μάθετε πώς](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3.    Εάν το Office είναι ήδη εγκατεστημένο στο διακομιστή RDS χρησιμοποιώντας οποιεσδήποτε άλλες συνδρομές της Microsoft, καταργήστε την εγκατάστασή του. Για παράδειγμα, μεταβαίνωσε **στον Πίνακα Ελέγχου**Κατάργηση εγκατάστασης ενός  >  **προγράμματος**. Καταργήστε την εγκατάσταση [χρησιμοποιώντας το Βοηθό υποστήριξης και αποκατάστασης της Microsoft,](https://aka.ms/SARA-OfficeUninstall-Alchemy) εάν εξαντλείστε προβλήματα.
4.    Στο διακομιστή RDS, συνδεθείτε στο κέντρο διαχείρισης του Microsoft 365 με το λογαριασμό διαχειριστή και [εγκαταστήστε τις Εφαρμογές Microsoft 365 για μεγάλες επιχειρήσεις](https://portal.office.com/OLS/MySoftware.aspx).
5.    Μετά την εγκατάσταση του Office, ***μην ανοίξετε ή εισέλθετε σε*** εφαρμογές του Office.
6.    Στο διακομιστή RDS, ενεργοποιήστε την ενεργοποίηση κοινόχρηστου υπολογιστή με επεξεργασία του μητρώου, ακολουθώντας τα εξής βήματα:
   1. Κάντε δεξί κλικ στο κουμπί των Windows στην κάτω αριστερή γωνία της οθόνης σας και επιλέξτε **Εκτέλεση**. Στο πλαίσιο Άνοιγμα , **πληκτρολογήστε regedit**και, στη συνέχεια, επιλέξτε **OK**.
   2. Επιλέξτε **Ναι** όταν σας ζητηθεί να επιτρέψετε στον Επεξεργαστή Μητρώου (Registry Editor) να κάνει αλλαγές στη συσκευή σας.
   3. Στον Επεξεργαστή Μητρώου (Registry Editor), προσθέστε μια τιμή συμβολοσειράς της **άδειας χρήσης κοινόχρηστου υπολογιστή** με ρύθμιση 1 υπό HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. Στο διακομιστή RDS, ***εισέλθετε ως τελικός χρήστης*** και [βεβαιωθείτε ότι είναι ενεργοποιημένη η ενεργοποίηση κοινόχρηστου υπολογιστή για εφαρμογές Microsoft 365 για επιχειρήσεις](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

