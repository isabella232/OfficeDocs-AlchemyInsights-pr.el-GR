---
title: Δεν είναι δυνατή η διαγραφή στοιχείων στο SharePoint ή OneDrive
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 21d7b928fade48a6729c120e6ea33b16dafe799e
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057716"
---
# <a name="unable-to-delete-items"></a>Δεν είναι δυνατή η διαγραφή στοιχείων

Αντιμετωπίζετε ζητήματα με τη διαγραφή στοιχείων;

- Πάντα βεβαιωθείτε ότι έχετε τα [κατάλληλα δικαιώματα](https://docs.microsoft.com/en-us/sharepoint/default-sharepoint-groups) για να διαγράψετε το στοιχείο ή να έχετε μια προσπάθεια [διαχειριστής συλλογής τοποθεσιών](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) , κατάργηση του στοιχείου.

- Βεβαιωθείτε ότι δεν υπάρχει μια ρύθμιση [πολιτικής διατήρησης](https://docs.microsoft.com/en-us/office365/securitycompliance/retention-policies) στο στοιχείο.

- Βεβαιωθείτε ότι το στοιχείο δεν είναι [ανάληψη ελέγχου](https://support.office.com/en-us/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) σε άλλο χρήστη.

- Τέλος, οι διαχειριστές μπορούν να χρησιμοποιούν [SharePoint μοτίβα και πρακτικές](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) που περιέχει μια βιβλιοθήκη του PowerShell εντολές που σας επιτρέπουν να εκτελέσετε ενέργειες διαχείρισης πολύπλοκων όπως επιβάλλει τη διαγραφή stubborn στοιχείων. 
- [Κατάργηση αρχείου Τοποθέτησης και Άμεσης Λειτουργίας](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Κατάργηση του φακέλου Τοποθέτησης και Άμεσης Λειτουργίας](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Κατάργηση στοιχείου λίστας Τοποθέτησης και Άμεσης Λειτουργίας](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Κατάργηση της λίστας Τοποθέτησης και Άμεσης Λειτουργίας](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Κατάργηση Τοποθέτησης και Άμεσης Λειτουργίας πεδίο (στήλη)](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)