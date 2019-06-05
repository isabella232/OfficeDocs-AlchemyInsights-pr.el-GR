---
title: Δημιουργία τοποθεσίας στο SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 2097933dd20f326a7bda2151596d514c37d566ff
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/04/2019
ms.locfileid: "34717767"
---
# <a name="create-sharepoint-sites-using-templates"></a>Δημιουργία τοποθεσιών του SharePoint, χρησιμοποιώντας τα πρότυπα

Τα πρότυπα τοποθεσίας του SharePoint είναι προκατασκευασμένες ορισμοί σχεδιασμένο γύρω από μια συγκεκριμένη επιχειρηματική ανάγκη. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα <a href="https://support.office.com/en-us/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4">χρησιμοποιώντας πρότυπα για να δημιουργήσετε διαφορετικά είδη των τοποθεσιών του SharePoint.</a></span></p> <p><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Ακολουθούν ορισμένα κοινά θέματα/λύσεις σχετικά με την αποθήκευση μιας τοποθεσίας ή λίστας ως πρότυπο στο Sharepoint Online.</span></p> <p><strong style="mso-bidi-font-weight: normal;"><u><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">"Πρότυπο" τοποθεσία/λίστα Αποθήκευση "δεν είναι διαθέσιμη ή δεν υπάρχει.</span></u></strong></p> <ul> <li><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Οι διαχειριστές θα πρέπει να επιτρέψει προσαρμοσμένης δέσμης ενεργειών για να ενεργοποιήσετε τις δυνατότητες του προτύπου. Για λεπτομερή βήματα, παραδείγματα και ζητήματα, δείτε </span> </span> <a style="orphans: 2; -webkit-text-stroke-width: 0px; word-spacing: 0px;" href="https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script">επιτρέπεται ή να απαγορεύεται η προσαρμοσμένη δέσμη ενεργειών</a>.</li> <li><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Την αποθήκευση τοποθεσίας ως πρότυπο εντολή δεν υποστηρίζεται και μπορεί να προκαλέσει προβλήματα σε τοποθεσίες που χρησιμοποιούν την υποδομή δημοσίευσης του SharePoint Server.</span></li> </ul> <p><strong style="mso-bidi-font-weight: normal;"><u><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Το πρότυπο τοποθεσίας δεν είναι δυνατό να δημιουργηθεί ή δεν λειτουργεί σωστά</span></u></strong></p> <ul> <li><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Το πρότυπο ενδέχεται να λείπει μια <a href="https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx">δυνατότητα</a> και κερδίσει&rsquo;t ενεργοποίηση. Εάν η δυνατότητα δεν είναι διαθέσιμη για την ενεργοποίηση της τρέχουσας συλλογής τοποθεσιών, μπορείτε να χρησιμοποιήσετε το πρότυπο τοποθεσίας για να δημιουργήσετε μια τοποθεσία.</span></li> <li><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Ελέγξτε για να δείτε εάν οποιεσδήποτε λίστες ή βιβλιοθήκες υπερβαίνουν το <a href="https://support.office.com/en-us/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59">Όριο το όριο προβολής λίστας των</a> 5000 στοιχεία όπως αυτό μπορεί να αποκλείσει τη δημιουργία ενός προτύπου τοποθεσίας.</span></li> <li><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Η τοποθεσία μπορεί να χρησιμοποιεί πάρα πολλούς πόρους και επομένως το πρότυπο τοποθεσίας υπερβαίνει το όριο των 50 MB.</span></li> <li>
Υπάρχουν προβλήματα που εμφανίζουν δεδομένα από μια λίστα που χρησιμοποιεί μια στήλη αναζήτησης. Για περισσότερες πληροφορίες, ανατρέξτε στην ενότητα </span> <span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;"> <a style="box-sizing: border-box; -webkit-text-stroke-width: 0px; word-spacing: 0px;" href="https://support.office.com/en-us/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a"> <span style="color: #0067b8; text-decoration: none; text-underline: none;">που δημιουργείται από το πρότυπο λίστας&rsquo;t εμφάνιση δεδομένων από τη λίστα αναζήτησης σωστά στο SharePoint Online.

Για πιο αναλυτικές πληροφορίες σχετικά με προβλήματα και λύσεις, ελέγξτε <a href="https://support.office.com/en-us/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989">δημιουργία και τη χρήση προτύπων τοποθεσίας.



