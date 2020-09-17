---
title: Δεν είναι δυνατή η διαγραφή στοιχείων στο SharePoint ή στο OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: fd12115214cc28b822cf7fa57fe9b86f76f7beb1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806111"
---
# <a name="unable-to-delete-items"></a>Δεν είναι δυνατή η διαγραφή στοιχείων

Οι πολιτικές διατήρησης μπορεί να προκαλέσουν αυτό το πρόβλημα, πρέπει είτε να απενεργοποιήσετε είτε να εξαιρέσετε τη σχετική αναμονή που προκαλεί αυτό το πρόβλημα. Μετά την κατάργηση μιας πολιτικής διατήρησης ή μιας διατήρησης, μπορεί να χρειαστούν έως και 24 ώρες για να ισχύσει η αλλαγή. Βεβαιωθείτε ότι δεν υπάρχει ρύθμιση [πολιτικής διατήρησης](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) στο στοιχείο.

Η τοποθεσία μπορεί να έχει υπερβεί το όριο χώρου αποθήκευσης, να αυξήσει το όριο της [τοποθεσίας](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) και να διαγράψει το στοιχείο.

Βεβαιωθείτε ότι δεν έχει γίνει [ανάληψη ελέγχου](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) του στοιχείου σε άλλο χρήστη.

Τέλος, οι διαχειριστές μπορούν να χρησιμοποιούν [μοτίβα και πρακτικές του SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP), τα οποία περιέχουν εντολές του PowerShell, οι οποίες σας επιτρέπουν να εκτελείτε σύνθετες ενέργειες διαχείρισης, όπως η υποχρεωτική Διαγραφή επίμονων στοιχείων.
- [Κατάργηση αρχείου PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Κατάργηση φακέλου τοποθέτησης και άμεσης λειτουργίας](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Κατάργηση στοιχείου λίστας τοποθέτησης και άμεσης λειτουργίας](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Κατάργηση λίστας τοποθέτησης και άμεσης λειτουργίας](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Κατάργηση πεδίου τοποθέτησης και άμεσης λειτουργίας (στήλη)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)