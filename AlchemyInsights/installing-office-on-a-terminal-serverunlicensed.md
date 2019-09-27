---
title: Εγκατάσταση του Office σε διακομιστή τερματικού-χωρίς άδεια χρήσης
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
ms.openlocfilehash: 51d1a66fdf9774bbe58bfdbe89317bc93834be09
ms.sourcegitcommit: 5e6a805fb0b41d714ca1cf90e23b8e2daa90f90e
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37205409"
---
# <a name="installing-office-on-a-terminal-server"></a>Εγκατάσταση του Office σε διακομιστή τερματικού

Για την ανάπτυξη του Office 365 ProPlus σε ένα διακομιστή των Windows χρησιμοποιώντας υπηρεσίες απομακρυσμένης επιφάνειας εργασίας (RDS), παλαιότερα ονομαζόταν υπηρεσίες Terminal Services:
  
- Πρέπει να έχετε ένα σχέδιο 365 του Office που περιλαμβάνει το Office 365 ProPlus, όπως το Office 365 Enterprise ε ή Enterprise Ε+. Τα σχέδια Office 365 Business και Office 365 Business Premium δεν περιλαμβάνουν το Office 365 ProPlus.

- Πρέπει να ενεργοποιήσετε την [Ενεργοποίηση του κοινόχρηστου υπολογιστή](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

Εάν θέλετε να εγκαταστήσετε το Office 365 ProPlus σε RDS από το κέντρο διαχείρισης της Microsoft 365, το ***οποίο χρησιμοποιεί τις προεπιλεγμένες ρυθμίσεις εγκατάστασης***, ακολουθήστε τα παρακάτω βήματα.

> [!TIP]
> Μπορείτε επίσης να κάνετε λήψη και εκτέλεση του [βοηθού υποστήριξης της Microsoft και αποκατάστασης](https://aka.ms/SaRA_OfficeSCA_M365Portal) για να εγκαταστήσετε το Office 365 ProPlus σε λειτουργία κοινής χρήσης υπολογιστή.
  
1. Ελέγξτε το σχέδιο 365 του Office που έχετε. [Μάθετε πώς](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. Εάν είναι απαραίτητο, μεταβείτε σε διαφορετικό σχέδιο του Office 365. [Μάθετε πώς](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. Εάν το Office είναι ήδη εγκατεστημένο στο διακομιστή RDS χρησιμοποιώντας οποιαδήποτε άλλα σχέδια του Office 365, απεγκαταστήστε το. Για παράδειγμα, πηγαίνοντας στον πίνακα \> ελέγχου απεγκατάσταση ενός προγράμματος. Κατάργηση εγκατάστασης χρησιμοποιώντας [την υποστήριξη της Microsoft και τον βοηθό αποκατάστασης](https://aka.ms/SARA-OfficeUninstall-Alchemy) , εάν εκτελείτε ζητήματα.

4. Στο διακομιστή RDS, εισέλθετε στο κέντρο διαχείρισης Microsoft 365 με το λογαριασμό διαχειριστή σας και εγκαταστήστε το [Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).

5. Μετά την εγκατάσταση του Office, ***Μην ανοίξετε ή εισέλθετε*** σε οποιεσδήποτε εφαρμογές του Office.

6. Στο διακομιστή RDS, ενεργοποιήστε την ενεργοποίηση του κοινόχρηστου υπολογιστή με την επεξεργασία του μητρώου, ακολουθώντας τα εξής βήματα:

1. Κάντε δεξιό κλικ στο κουμπί των Windows στην κάτω αριστερή γωνία της οθόνης σας και επιλέξτε εκτέλεση. Στο πλαίσιο Άνοιγμα, πληκτρολογήστε **regedit**και, στη συνέχεια, επιλέξτε OK.

2. Επιλέξτε Yes όταν σας ζητηθεί να επιτρέψετε στον επεξεργαστή μητρώου να κάνει αλλαγές στη συσκευή σας.

3. Στο πρόγραμμα επεξεργασίας μητρώου, προσθέστε μια τιμή συμβολοσειράς της κοινής **χρήσης υπολογιστή** με ρύθμιση 1 κάτω από το HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office

7. Στο διακομιστή RDS, ***εισέλθετε ως τελικός χρήστης*** και [Επιβεβαιώστε ότι η ενεργοποίηση του κοινόχρηστου υπολογιστή είναι ενεργοποιημένη για το Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

Για περισσότερες λεπτομέρειες σχετικά με τις προϋποθέσεις, οδηγίες εγκατάστασης και οδηγίες σχετικά με προσαρμοσμένες εγκαταστάσεις, χρησιμοποιώντας το εργαλείο ανάπτυξης του Office, ανατρέξτε στην ενότητα [ανάπτυξη Office 365 ProPlus, χρησιμοποιώντας τις υπηρεσίες απομακρυσμένης επιφάνειας εργασίας](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
Για να διορθώσετε σφάλματα που σχετίζονται με την ενεργοποίηση του κοινόχρηστου υπολογιστή, ανατρέξτε στο [θέμα Αντιμετώπιση προβλημάτων με την ενεργοποίηση του κοινόχρηστου υπολογιστή για το Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  