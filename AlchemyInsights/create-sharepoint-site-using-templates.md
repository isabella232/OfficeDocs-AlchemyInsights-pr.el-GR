---
title: Δημιουργία τοποθεσίας στο SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b9009fdbdc2a5e7443151446daade1685d2f5d45
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770423"
---
# <a name="create-sharepoint-sites-using-templates"></a>Δημιουργία τοποθεσιών του SharePoint με χρήση προτύπων

Η δυνατότητα αποθήκευσης μιας τοποθεσίας ως προτύπου δεν υποστηρίζεται με σύγχρονες επικοινωνίες ή τοποθεσίες ομάδων. Για περισσότερες πληροφορίες σχετικά με τη χρήση προτύπων [, ανατρέξτε στο θέμα Αποθήκευση, λήψη και αποστολή τοποθεσίας SharePoint ως προτύπου](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).

Ακολουθούν ορισμένα συνηθισμένα ζητήματα/λύσεις σχετικά με την αποθήκευση μιας τοποθεσίας ή λίστας ως προτύπου στο SharePoint Online. 

**Η αποθήκευση του κουμπιού "πρότυπο τοποθεσίας/λίστας" δεν είναι διαθέσιμη ή λείπει**

Οι διαχειριστές θα πρέπει να επιτρέψουν προσαρμοσμένη δέσμη ενεργειών για να ενεργοποιήσετε τις δυνατότητες του προτύπου. Για αναλυτικά βήματα, παραδείγματα και παρατηρήσεις Δείτε 

- [Αποδοχή ή αποτροπή προσαρμοσμένης δέσμης ενεργειών](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Η εντολή "Αποθήκευση τοποθεσίας ως προτύπου" δεν υποστηρίζεται και μπορεί να προκαλέσει προβλήματα σε τοποθεσίες που χρησιμοποιούν την υποδομή δημοσίευσης του SharePoint Server.

**Δεν είναι δυνατή η δημιουργία του προτύπου τοποθεσίας ή δεν λειτουργεί σωστά**

Το πρότυπο μπορεί να λείπει μια [δυνατότητα](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) και δεν θα ενεργοποιηθεί. Εάν η δυνατότητα δεν είναι διαθέσιμη για ενεργοποίηση στην τρέχουσα συλλογή τοποθεσιών, δεν μπορείτε να χρησιμοποιήσετε το πρότυπο τοποθεσίας για να δημιουργήσετε μια τοποθεσία.

- Ελέγξτε αν οποιεσδήποτε λίστες ή βιβλιοθήκες υπερβαίνουν το όριο [προβολής λίστας](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) των 5000 στοιχείων, καθώς αυτό μπορεί να εμποδίσει τη δημιουργία ενός προτύπου τοποθεσίας.

- Η τοποθεσία μπορεί να χρησιμοποιεί πάρα πολλούς πόρους και, επομένως, το πρότυπο τοποθεσίας υπερβαίνει το όριο 50 MB.


- Υπάρχουν προβλήματα στην εμφάνιση δεδομένων από μια λίστα που χρησιμοποιεί μια στήλη αναζήτησης. Για περισσότερες πληροφορίες, ανατρέξτε στο [πρότυπο λίστα που δημιουργήθηκε δεν εμφανίζει δεδομένα από τη λίστα αναζήτησης σωστή στο SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

Για πιο λεπτομερείς πληροφορίες σχετικά με κοινά προβλήματα και λύσεις, ελέγξτε τη [δημιουργία και χρήση προτύπων τοποθεσίας](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



