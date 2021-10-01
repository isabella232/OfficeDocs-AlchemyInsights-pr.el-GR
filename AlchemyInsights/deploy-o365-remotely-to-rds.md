---
title: Ανάπτυξη Εφαρμογές Microsoft 365 για κοινόχρηστη χρήση σε RDS, Terminal Server ή VDI
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
ms.openlocfilehash: 81183cf1823480c1b15eba9ba9f519b4e3746b52
ms.sourcegitcommit: ef8d6b71fbd962fb3f7081b21724e67a91111a92
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 10/01/2021
ms.locfileid: "60077250"
---
# <a name="deploying-microsoft-365-apps-for-shared-use-on-rds-terminal-server-or-vdi"></a>Ανάπτυξη Εφαρμογές Microsoft 365 για κοινόχρηστη χρήση σε RDS, Terminal Server ή VDI

Για να αναπτύξετε Εφαρμογές Microsoft 365 χρησιμοποιώντας τις Υπηρεσίες απομακρυσμένης επιφάνειας εργασίας (RDS), πρώην Υπηρεσίες τερματικού, πρέπει να κάνετε τα εξής:

- Χρησιμοποιήστε την εύκολη επιδιόρθωση για να ενεργοποιήσετε το TLS 1.2 ως προεπιλογή, εάν χρησιμοποιείτε μια παλαιότερη έκδοση του Windows (π.χ. Windows 7 SP1, Windows Server 2008 R2). Για εύκολη επιδιόρθωση και περισσότερες πληροφορίες, ανατρέξτε στο θέμα Ενημέρωση για την ενεργοποίηση των [TLS 1.1 και TLS 1.2 ως προεπιλεγμένων ασφαλών πρωτοκόλλων στο WinHTTP στο Windows.](https://support.microsoft.com/en-us/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392#bkmk_easy) 
- Να έχετε ένα πρόγραμμα που περιλαμβάνει το Εφαρμογές Microsoft 365 για μεγάλες επιχειρήσεις (προηγουμένως Office 365 Plus). Για παράδειγμα, Office 365 E3 ή Microsoft 365 E5 ή οποιοδήποτε πρόγραμμα που περιλαμβάνει την έκδοση υπολογιστή του Project ή του Visio, όπως Project Πρόγραμμα 3 ή Visio Πρόγραμμα 2, ή το πρόγραμμα Microsoft 365 Premium για Επιχειρήσεις, το οποίο περιλαμβάνει επίσης Εφαρμογές Microsoft 365 για επιχειρήσεις.
- Ενεργοποίηση ενεργοποίησης κοινόχρηστου υπολογιστή. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Επισκόπηση της ενεργοποίησης κοινόχρηστων υπολογιστών για Εφαρμογές Microsoft 365.](https://docs.microsoft.com/deployoffice/overview-shared-computer-activation)

**Σημείωση:** Για να εγκαταστήσετε Εφαρμογές Microsoft 365 σε λειτουργία ενεργοποίησης κοινόχρηστου υπολογιστή, κάντε λήψη και εκτέλεση του [προγράμματος Βοηθός υποστήριξης και αποκατάστασης Microsoft.](https://aka.ms/SaRA_OfficeSCA_M365Portal) Για λεπτομέρειες σχετικά με τα προαπαιτούμενα στοιχεία, τις οδηγίες εγκατάστασης και τις οδηγίες για την προσαρμογή των εγκαταστάσεων με χρήση του Εργαλείου ανάπτυξης Office, ανατρέξτε στο θέμα [Ανάπτυξη Εφαρμογές Microsoft 365 με χρήση των υπηρεσιών απομακρυσμένης επιφάνειας εργασίας.](https://docs.microsoft.com/deployoffice/deploy-microsoft-365-apps-remote-desktop-services)

Για να διορθώσετε σφάλματα που σχετίζονται με την ενεργοποίηση σε κοινόχρηστο υπολογιστή, ανατρέξτε στα θέματα:

- [Αντιμετώπιση προβλημάτων με την ενεργοποίηση κοινόχρηστου υπολογιστή για Εφαρμογές Microsoft 365](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation)
- [Επαναφορά κατάστασης ενεργοποίησης Εφαρμογές Microsoft 365 για μεγάλες επιχειρήσεις](https://docs.microsoft.com/office/troubleshoot/activation/reset-office-365-proplus-activation-state)

Εάν θέλετε να εγκαταστήσετε Εφαρμογές Microsoft 365 σε RDS από το Κέντρο διαχείρισης Microsoft 365, το οποίο χρησιμοποιεί προεπιλεγμένες ρυθμίσεις εγκατάστασης, ακολουθήστε τα παρακάτω βήματα:

1. Ελέγξτε τι Microsoft 365 πρόγραμμα έχετε. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Ποια συνδρομή έχω;](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).

1. Εάν είναι απαραίτητο, αλλάξτε σε διαφορετικό πρόγραμμα Microsoft 365. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Αναβάθμιση σε διαφορετικό πρόγραμμα.](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan)

1. Εάν Εφαρμογές Microsoft 365 είναι ήδη εγκατεστημένο στον διακομιστή RDS χρησιμοποιώντας οποιαδήποτε άλλα μη συμβατά προγράμματα, καταργήστε την εγκατάστασή του από **τον Πίνακα**  >  **Ελέγχου.** Εάν αντιμετωπίσετε προβλήματα, καταργήστε την εγκατάσταση με τη λήψη [του Microsoft Βοηθός υποστήριξης και αποκατάστασης](https://aka.ms/SARA-OfficeUninstall-Alchemy).

1. Στο διακομιστή RDS, πραγματοποιήστε είσοδο στο Κέντρο διαχείρισης Microsoft 365 με το λογαριασμό διαχειριστή σας και [εγκαταστήστε το Office](https://portal.office.com/OLS/MySoftware.aspx).

   Μετά την εγκατάσταση του Office, μην ανοίγετε ούτε εισέλθετε σε εφαρμογές Office.

1. Στο διακομιστή RDS, ενεργοποιήστε την ενεργοποίηση του κοινόχρηστου υπολογιστή κάνοντας επεξεργασία του μητρώου:

   1. Κάντε δεξί κλικ στο κουμπί Windows στην κάτω αριστερή γωνία της οθόνης σας και επιλέξτε **Εκτέλεση.** Στο πλαίσιο Άνοιγμα, πληκτρολογήστε **regedit** και, στη συνέχεια, επιλέξτε **OK**.

   1. Όταν σας ζητηθεί να επιτρέψετε στον Επεξεργαστή μητρώου να κάνει αλλαγές στη συσκευή σας, επιλέξτε **Ναι.**

   1. Στον Επεξεργαστή Μητρώου, στην περιοχή HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration, προσθέστε μια τιμή συμβολοσειράς **"SharedComputerLicensing"** με ρύθμιση **1.**

1. Στο διακομιστή RDS, πραγματοποιήστε είσοδο ως τελικός χρήστης και βεβαιωθείτε ότι η ενεργοποίηση κοινόχρηστου υπολογιστή είναι ενεργοποιημένη για Εφαρμογές Microsoft 365. 

   Για λεπτομέρειες, ανατρέξτε στο θέμα [Επαλήθευση ότι η ενεργοποίηση σε κοινόχρηστο υπολογιστή είναι ενεργοποιημένη για Εφαρμογές Microsoft 365.](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation#verify-that-shared-computer-activation-is-enabled-for-microsoft-365-apps)