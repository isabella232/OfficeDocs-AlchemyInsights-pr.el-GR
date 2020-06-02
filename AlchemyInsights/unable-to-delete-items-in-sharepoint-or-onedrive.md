---
title: Δεν είναι δυνατή η διαγραφή στοιχείων στο SharePoint ή το OneDrive
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
ms.openlocfilehash: 8647b65c52a782ca48ca58bb2700556db528796b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511976"
---
# <a name="unable-to-delete-items"></a>Δεν είναι δυνατή η διαγραφή στοιχείων

Οι πολιτικές διατήρησης μπορεί να προκαλέσουν αυτό, πρέπει είτε να απενεργοποιήσετε είτε να εξαιρέσετε την αντίστοιχη διατήρηση που προκαλεί αυτό το ζήτημα. Μετά την κατάργηση μιας πολιτικής διατήρησης ή διατήρησης, ενδέχεται να χρειαστούν έως και 24 ώρες για να εφαρμοστεί η αλλαγή. Βεβαιωθείτε ότι δεν υπάρχει ρύθμιση [πολιτικής διατήρησης](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) στο στοιχείο.

Η τοποθεσία ενδέχεται να έχει υπερβεί το όριο αποθήκευσης, να αυξήσει το [όριο τοποθεσίας](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) και να διαγράψει το στοιχείο.

Βεβαιωθείτε ότι δεν έχει γίνει ανάληψη ελέγχου του [στοιχείου](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) σε άλλο χρήστη.

Τέλος, οι διαχειριστές μπορούν να [χρησιμοποιήσουν μοτίβα και πρακτικές του SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP), η οποία περιέχει μια βιβλιοθήκη εντολών PowerShell που σας επιτρέπουν να εκτελείτε σύνθετες ενέργειες διαχείρισης, όπως η σταδιακή διαγραφή επίμονων στοιχείων.
- [Κατάργηση αρχείου PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Κατάργηση φακέλου PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Κατάργηση στοιχείου λίστας PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Κατάργηση λίστας PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Κατάργηση πεδίου PNP (Στήλη)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)