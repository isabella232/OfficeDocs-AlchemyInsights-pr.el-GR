---
title: Ανάπτυξη του Office 365 ProPlus για κοινή χρήση σε RDS, διακομιστή τερματικού ή ΗΣ
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 12/9/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 2312cca9ebf5dad1322bc98335cef6a6bc81f03e
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959460"
---
# <a name="deploying-office-365-proplus-for-shared-use-on-rds-terminal-server-or-vdi"></a>Ανάπτυξη του Office 365 ProPlus για κοινή χρήση σε RDS, διακομιστή τερματικού ή ΗΣ

Για να αναπτύξετε το Office 365 ProPlus χρησιμοποιώντας τις υπηρεσίες απομακρυσμένης επιφάνειας εργασίας (RDS), που παλαιότερα ονομαζόταν υπηρεσίες Terminal Services:
- Πρέπει να έχετε ένα πρόγραμμα Microsoft 365 για επαγγελματική ή ένα πρόγραμμα του Office 365 που περιλαμβάνει το Office 365 ProPlus, όπως το Office 365 Enterprise ε ή Enterprise ε+.
   > [!NOTE] 
   > Τα σχέδια Office 365 Business και Office 365 Business Premium δεν περιλαμβάνουν το Office 365 ProPlus.
- Πρέπει να ενεργοποιήσετε την [Ενεργοποίηση του κοινόχρηστου υπολογιστή](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

> [!NOTE]
> Μπορείτε επίσης να κάνετε λήψη και εκτέλεση του [βοηθού υποστήριξης της Microsoft και αποκατάστασης](https://aka.ms/SaRA_OfficeSCA_M365Portal) για να εγκαταστήσετε το Office 365 ProPlus σε λειτουργία κοινής χρήσης υπολογιστή.

Για περισσότερες πληροφορίες σχετικά με τις προϋποθέσεις, οδηγίες εγκατάστασης και οδηγίες σχετικά με προσαρμοσμένες εγκαταστάσεις, χρησιμοποιώντας το εργαλείο ανάπτυξης του Office, ανατρέξτε στην ενότητα [ανάπτυξη του office 365 ProPlus χρησιμοποιώντας τις υπηρεσίες απομακρυσμένης επιφάνειας εργασίας](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).

Για να διορθώσετε σφάλματα που σχετίζονται με την ενεργοποίηση κοινόχρηστου υπολογιστή:
- Δείτε [Αντιμετώπιση προβλημάτων με την ενεργοποίηση του κοινόχρηστου υπολογιστή για το Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
- Δείτε [Επαναφορά κατάστασης ενεργοποίησης του Office 365 ProPlus](https://go.microsoft.com/fwlink/?linkid=2109218).

Εάν θέλετε να εγκαταστήσετε το Office 365 ProPlus σε RDS από το κέντρο διαχείρισης της Microsoft 365, το ***οποίο χρησιμοποιεί τις προεπιλεγμένες ρυθμίσεις εγκατάστασης***, ακολουθήστε τα εξής βήματα:

1.  Ελέγξτε το σχέδιο 365 του Office που έχετε. [Μάθε πώς](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).
2.  Εάν είναι απαραίτητο, μεταβείτε σε διαφορετικό σχέδιο του Office 365. [Μάθε πώς](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).
3.  Εάν το Office είναι ήδη εγκατεστημένο στο διακομιστή RDS χρησιμοποιώντας οποιαδήποτε άλλα σχέδια του Office 365, απεγκαταστήστε το. Για παράδειγμα, πηγαίνοντας στον **πίνακα** > ελέγχου**απεγκαταστήσετε ένα πρόγραμμα**. Κατάργηση εγκατάστασης χρησιμοποιώντας [την υποστήριξη της Microsoft και τον βοηθό αποκατάστασης](https://aka.ms/SARA-OfficeUninstall-Alchemy) , εάν εκτελείτε ζητήματα.
4.  Στο διακομιστή RDS, εισέλθετε στο κέντρο διαχείρισης Microsoft 365 με το λογαριασμό διαχειριστή σας και εγκαταστήστε το [Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).
5.  Μετά την εγκατάσταση του Office, ***Μην ανοίξετε ή εισέλθετε*** σε οποιεσδήποτε εφαρμογές του Office.
6.  Στο διακομιστή RDS, ενεργοποιήστε την ενεργοποίηση του κοινόχρηστου υπολογιστή με την επεξεργασία του μητρώου, ακολουθώντας τα εξής βήματα:
   1. Κάντε δεξιό κλικ στο κουμπί των Windows στην κάτω αριστερή γωνία της οθόνης σας και επιλέξτε **εκτέλεση**. Στο πλαίσιο Άνοιγμα, πληκτρολογήστε **regedit**και, στη συνέχεια, επιλέξτε **OK**.
   2. Επιλέξτε **Yes** όταν σας ζητηθεί να επιτρέψετε στον επεξεργαστή μητρώου να κάνει αλλαγές στη συσκευή σας.
   3. Στον επεξεργαστή μητρώου, προσθέστε μια τιμή συμβολοσειράς του προγράμματος **Υπολογιστέςάδειας χρήσης** με μια ρύθμιση 1 κάτω από HKEY_LOCAL_MACHINE \Softpares\doot\soot\ \ Ρυθμίσεις \ Microsoft \ Office.
   4. Στο διακομιστή RDS, ***εισέλθετε ως τελικός χρήστης*** και [Επιβεβαιώστε ότι η ενεργοποίηση του κοινόχρηστου υπολογιστή είναι ενεργοποιημένη για το Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

