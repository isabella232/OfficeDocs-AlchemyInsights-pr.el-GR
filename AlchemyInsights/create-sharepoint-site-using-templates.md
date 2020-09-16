---
title: Δημιουργία τοποθεσίας στο SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b554bfa4ccccbd68d0c3df27cf17397f860735c2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732224"
---
# <a name="create-sharepoint-sites-using-templates"></a>Δημιουργία τοποθεσιών του SharePoint με χρήση προτύπων

Η δυνατότητα αποθήκευσης μιας τοποθεσίας ως προτύπου δεν υποστηρίζεται από τις σύγχρονες επικοινωνίες ή τις τοποθεσίες ομάδας. Για περισσότερες πληροφορίες σχετικά με τη χρήση προτύπων [, ανατρέξτε στο θέμα Αποθήκευση, λήψη και αποστολή μιας τοποθεσίας του SharePoint ως προτύπου](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).

Ακολουθούν ορισμένα συνηθισμένα προβλήματα/λύσεις σχετικά με την αποθήκευση μιας τοποθεσίας ή μιας λίστας ως προτύπου στο SharePoint Online. 

**Το κουμπί "Αποθήκευση προτύπου τοποθεσίας/λίστας" δεν είναι διαθέσιμο ή λείπει**

Οι διαχειριστές θα πρέπει να επιτρέψουν την προσαρμοσμένη δέσμη ενεργειών για να ενεργοποιήσουν τις δυνατότητες του προτύπου. Για λεπτομερή βήματα, παραδείγματα και θέματα, ανατρέξτε στο θέμα 

- [Αποδοχή ή αποτροπή προσαρμοσμένης δέσμης ενεργειών](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Η εντολή "Αποθήκευση τοποθεσίας ως προτύπου" δεν υποστηρίζεται και μπορεί να προκαλέσει προβλήματα σε τοποθεσίες που χρησιμοποιούν την υποδομή δημοσίευσης του SharePoint Server.

**Το πρότυπο τοποθεσίας δεν μπορεί να δημιουργηθεί ή δεν λειτουργεί σωστά**

Το πρότυπο μπορεί να λείπει από μια [δυνατότητα](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) και να μην ενεργοποιείται. Εάν η δυνατότητα δεν είναι διαθέσιμη για ενεργοποίηση στην τρέχουσα συλλογή τοποθεσιών, δεν μπορείτε να χρησιμοποιήσετε το πρότυπο τοποθεσίας για να δημιουργήσετε μια τοποθεσία.

- Βεβαιωθείτε ότι οι λίστες ή οι βιβλιοθήκες υπερβαίνουν το όριο [ορίου προβολής λίστας](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) των στοιχείων του 5000, καθώς αυτό μπορεί να αποκλείσει τη δημιουργία ενός προτύπου τοποθεσίας.

- Η τοποθεσία μπορεί να χρησιμοποιεί πάρα πολλούς πόρους και, επομένως, το πρότυπο τοποθεσίας υπερβαίνει το όριο του 50 MB.


- Υπάρχουν προβλήματα με την εμφάνιση δεδομένων από μια λίστα που χρησιμοποιεί μια στήλη αναζήτησης. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [η λίστα που δημιουργήθηκε με πρότυπο δεν εμφανίζει δεδομένα από τη σωστή λίστα αναζήτησης στο SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

Για πιο λεπτομερείς πληροφορίες σχετικά με τα συνηθισμένα προβλήματα και λύσεις, ανατρέξτε στο θέμα [δημιουργία και χρήση προτύπων τοποθεσίας](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



