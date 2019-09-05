---
title: Δεν είναι δυνατή η διαγραφή στοιχείων στο SharePoint ή στο OneDrive
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 3cc168846999c6880b95edfaedb2df8cf6e843a6
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36748555"
---
# <a name="unable-to-delete-items"></a>Δεν είναι δυνατή η διαγραφή στοιχείων

Αντιμετωπίζετε προβλήματα με τη διαγραφή στοιχείων του SharePoint;

- Να είστε πάντα βέβαιοι ότι έχετε τα [κατάλληλα δικαιώματα](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) για να διαγράψετε το στοιχείο ή ότι ένας [διαχειριστής συλλογής τοποθεσιών](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) επιχειρεί να καταργήσει το στοιχείο.

- Βεβαιωθείτε ότι δεν υπάρχει ρύθμιση [πολιτικής διατήρησης](https://docs.microsoft.com/office365/securitycompliance/retention-policies) στο στοιχείο.

- Βεβαιωθείτε ότι το στοιχείο δεν έχει γίνει [ανάληψη ελέγχου](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) σε άλλο χρήστη.

- Τέλος, οι διαχειριστές μπορούν να χρησιμοποιούν το [SharePoint μοτίβα και πρακτικές](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) που περιέχει μια βιβλιοθήκη των εντολών PowerShell που σας επιτρέπουν να εκτελέσετε σύνθετες ενέργειες διαχείρισης, όπως η αναγκαστική Διαγραφή πεισματική στοιχεία.
- [Κατάργηση αρχείου PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Κατάργηση φακέλου PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Κατάργηση στοιχείου λίστας PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Κατάργηση λίστας PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Κατάργηση πεδίου PNP (στήλη)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)