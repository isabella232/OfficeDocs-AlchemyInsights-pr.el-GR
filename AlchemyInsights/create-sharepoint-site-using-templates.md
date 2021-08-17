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
ms.openlocfilehash: eaf09aebad5568aab3a716ce28c8ce3357c9f43175e1b1458bfcd43fd95a71fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057966"
---
# <a name="create-sharepoint-sites-using-templates"></a>Δημιουργία SharePoint τοποθεσιών χρησιμοποιώντας πρότυπα

Η δυνατότητα αποθήκευσης μιας τοποθεσίας ως προτύπου δεν υποστηρίζεται με τις σύγχρονες τοποθεσίες επικοινωνίας ή ομάδας. Για περισσότερες πληροφορίες σχετικά με τη χρήση προτύπων, ανατρέξτε στο θέμα [Αποθήκευση, λήψη και αποστολή SharePoint τοποθεσίας ως προτύπου.](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template)

Ακολουθούν ορισμένα συνηθισμένα προβλήματα/λύσεις σχετικά με την αποθήκευση μιας τοποθεσίας ή λίστας ως προτύπου στο Sharepoint Online. 

**Το κουμπί "Αποθήκευση τοποθεσίας/προτύπου λίστας" δεν είναι διαθέσιμο ή λείπει**

Οι διαχειριστές θα πρέπει να επιτρέψουν την προσαρμοσμένη δέσμη ενεργειών για να ενεργοποιήσουν τις δυνατότητες του προτύπου. Για λεπτομερή βήματα, ανατρέξτε στα παραδείγματα και τα θέματα 

- [Αποδοχή ή αποτροπή προσαρμοσμένης δέσμης ενεργειών](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Η εντολή "Αποθήκευση τοποθεσίας ως προτύπου" δεν υποστηρίζεται και μπορεί να προκαλέσει προβλήματα σε τοποθεσίες που χρησιμοποιούν την SharePoint υποδομής δημοσίευσης διακομιστή.

**Δεν είναι δυνατή η δημιουργία ή η σωστή λειτουργία του προτύπου τοποθεσίας**

Ενδέχεται να λείπει μια δυνατότητα [από το πρότυπο](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) και να μην ενεργοποιείται. Εάν η δυνατότητα δεν είναι διαθέσιμη για ενεργοποίηση στην τρέχουσα συλλογή τοποθεσιών, δεν μπορείτε να χρησιμοποιήσετε το πρότυπο τοποθεσίας για να δημιουργήσετε μια τοποθεσία.

- Ελέγξτε εάν οποιεσδήποτε λίστες ή [](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) βιβλιοθήκες υπερβαίνουν το όριο ορίου προβολής λίστας των 5.000 στοιχείων, καθώς αυτό μπορεί να αποκλείσει τη δημιουργία ενός προτύπου τοποθεσίας.

- Η τοποθεσία μπορεί να χρησιμοποιεί πάρα πολλούς πόρους και, επομένως, το πρότυπο τοποθεσίας υπερβαίνει το όριο των 50 MB.


- Υπάρχουν προβλήματα με την εμφάνιση δεδομένων από μια λίστα που χρησιμοποιεί μια στήλη αναζήτησης. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα Η λίστα που δημιουργείται από πρότυπα δεν εμφανίζει δεδομένα από τη [σωστή λίστα αναζήτησης στο SharePoint Online.](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data)

Για πιο λεπτομερείς πληροφορίες σχετικά με συνήθη προβλήματα και λύσεις, ανατρέξτε στο πλαίσιο ["Δημιουργία και χρήση προτύπων τοποθεσίας".](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)



