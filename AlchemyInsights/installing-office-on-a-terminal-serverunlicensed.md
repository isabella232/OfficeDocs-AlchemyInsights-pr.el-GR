---
title: Την εγκατάσταση του office σε ένα διακομιστή τερματικού - χωρίς άδεια χρήσης
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 73d5128b55cae7712c48be9e2d05e558c3ba2e5c
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29471239"
---
# <a name="installing-office-on-a-terminal-server"></a>Την εγκατάσταση του Office σε ένα διακομιστή τερματικού

Για την ανάπτυξη του Office 365 ProPlus σε ένα διακομιστή των Windows χρησιμοποιώντας τις υπηρεσίες απομακρυσμένης επιφάνειας εργασίας (RDS), παλιότερα με το όνομα των υπηρεσιών Terminal Services:
  
- Πρέπει να έχετε ένα πρόγραμμα Office 365 που περιλαμβάνει το Office 365 ProPlus, όπως E3 Enterprise του Office 365 ή εταιρικού E5. Τα σχέδια Office 365 επιχειρήσεων και πριμοδότηση επαγγελματική του Office 365 δεν περιλαμβάνουν Office 365 ProPlus.
    
- Πρέπει να ενεργοποιήσετε την [Ενεργοποίηση κοινόχρηστο υπολογιστή](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).
    
Εάν θέλετε να εγκαταστήσετε το Office 365 ProPlus σε RDS από την πύλη Office 365, ** *που χρησιμοποιούν τις προεπιλεγμένες ρυθμίσεις εγκατάστασης* **, ακολουθήστε τα εξής βήματα: 
  
1. Ελέγξτε τι σχέδιο Office 365 που έχετε. [Μάθετε πώς](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)
    
2. Εάν είναι απαραίτητο, μεταβείτε σε ένα διαφορετικό Office 365 σχεδιασμό. [Μάθετε πώς](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)
    
3. Αν το Office είναι ήδη εγκατεστημένο στο διακομιστή RDS, χρησιμοποιώντας οποιαδήποτε άλλα σχέδια Office 365, καταργήσετε την εγκατάστασή του. Για παράδειγμα, μεταβαίνοντας τον πίνακα ελέγχου \> κατάργηση εγκατάστασης ενός προγράμματος. Καταργήστε την εγκατάσταση χρησιμοποιώντας την [υπηρεσία υποστήριξης της Microsoft και αποκατάστασης του Βοηθού](https://aka.ms/SARA-OfficeUninstall-Alchemy) εάν εκτελείτε σε θέματα. 
    
4. Στο διακομιστή RDS, εισέλθετε στην πύλη Office 365 με το λογαριασμό διαχειριστή και να [εγκαταστήσετε το Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).
    
5. Μετά την εγκατάσταση του Office, ** *δεν ανοίξετε ή να εισέλθετε* ** για τις εφαρμογές του Office. 
    
6. Στο διακομιστή RDS, δυνατή Ενεργοποίηση κοινόχρηστο υπολογιστή με επεξεργασία του μητρώου ακολουθώντας τα εξής βήματα:
    
1. Κάντε δεξιό κλικ στο κουμπί των Windows στην κάτω αριστερή γωνία της οθόνης σας και επιλέξτε εκτέλεση. Στο πλαίσιο Άνοιγμα, πληκτρολογήστε **regedit**και, στη συνέχεια, επιλέξτε OK. 
    
2. Επιλέξτε Ναι όταν σας ζητηθεί να επιτρέψετε τον Επεξεργαστή μητρώου για να κάνετε αλλαγές στη συσκευή σας.
    
3. Στον επεξεργαστή μητρώου, προσθέστε μια τιμή συμβολοσειράς **SharedComputerLicensing** με ρύθμιση 1 στην περιοχή HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration. 
    
7. Στο διακομιστή RDS, ** *εισέλθετε ως ένας τελικός χρήστης* ** και [Βεβαιωθείτε ότι είναι ενεργοποιημένη η ενεργοποίηση κοινόχρηστο υπολογιστή για Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).
    
Για περισσότερες λεπτομέρειες σχετικά με προϋποθέσεις, οδηγίες και κατευθύνσεις σχετικά με προσαρμοσμένες εγκαταστάσεις, χρησιμοποιώντας το εργαλείο ανάπτυξης του Office, ανατρέξτε [Αναπτύσσουν Office 365 ProPlus, χρησιμοποιώντας τις υπηρεσίες απομακρυσμένης επιφάνειας εργασίας](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
Για να διορθώσετε τα σφάλματα που αφορούν την ενεργοποίηση κοινόχρηστο υπολογιστή, ανατρέξτε στην [Αντιμετώπιση προβλημάτων με ενεργοποίηση κοινόχρηστο υπολογιστή για Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  

