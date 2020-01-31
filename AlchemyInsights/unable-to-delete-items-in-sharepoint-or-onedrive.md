---
title: Δεν είναι δυνατή η διαγραφή στοιχείων στο SharePoint ή στο OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: abfcb91c6040aeed759d697ca63546ccea8ede97
ms.sourcegitcommit: c5e800313a6f211386a384716e5fa18e7fcc8c1c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/28/2020
ms.locfileid: "41571255"
---
# <a name="unable-to-delete-items"></a>Δεν είναι δυνατή η διαγραφή στοιχείων

Πολιτικές διατήρησης μπορεί να προκαλέσει αυτό, θα πρέπει είτε να απενεργοποιήσετε ή να εξαιρέσετε αντίστοιχη λαβή που προκαλεί αυτό το ζήτημα. Αφού καταργηθεί η πολιτική διατήρησης ή η διατήρηση, ενδέχεται να χρειαστούν έως και 24 ώρες για να ισχύσει η αλλαγή. Βεβαιωθείτε ότι δεν υπάρχει ρύθμιση [πολιτικής διατήρησης](https://docs.microsoft.com/office365/securitycompliance/retention-policies) στο στοιχείο.

Η τοποθεσία μπορεί να έχει υπερβεί το όριο αποθήκευσης, να αυξήσει το όριο της [τοποθεσίας](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) και να διαγράψει το στοιχείο.

Βεβαιωθείτε ότι το στοιχείο δεν έχει γίνει [ανάληψη ελέγχου](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) σε άλλο χρήστη.

Τέλος, οι διαχειριστές μπορούν να χρησιμοποιήσουν το [SharePoint μοτίβα και πρακτικές](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) που περιέχει μια βιβλιοθήκη των εντολών PowerShell που σας επιτρέπουν να εκτελέσετε σύνθετες ενέργειες διαχείρισης, όπως η δύναμη Διαγραφή επίμονη στοιχεία.
- [Κατάργηση αρχείου PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Κατάργηση φακέλου τοποθέτησης και άμεσης λειτουργίας](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Κατάργηση στοιχείου λίστας τοποθέτησης και άμεσης λειτουργίας](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Κατάργηση λίστας τοποθέτησης και άμεσης λειτουργίας](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Κατάργηση πεδίου τοποθέτησης και άμεσης λειτουργίας (στήλη)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)