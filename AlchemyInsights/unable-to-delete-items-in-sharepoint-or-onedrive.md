---
title: Δεν είναι δυνατή η διαγραφή στοιχείων SharePoint ή OneDrive
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
ms.openlocfilehash: 3601c5eff121e10b6bddace6f7228204a01080a636e24f3a56373fe8d469c799
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038517"
---
# <a name="unable-to-delete-items"></a>Δεν είναι δυνατή η διαγραφή στοιχείων

- Οι πολιτικές διατήρησης μπορεί να προκαλέσουν αυτό το πρόβλημα, πρέπει να απενεργοποιήσετε ή να εξαιρέσετε την αντίστοιχη διατήρηση που προκαλεί αυτό το πρόβλημα. Μετά την κατάργηση μιας πολιτικής διατήρησης ή διατήρησης, ενδέχεται να χρειαστεί έως και 24 ώρες για την εφαρμογή της αλλαγής. Βεβαιωθείτε ότι δεν υπάρχει ρύθμιση [πολιτικής διατήρησης](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) στο στοιχείο.

- Η τοποθεσία μπορεί να έχει υπερβεί το όριο χώρου αποθήκευσης, να αυξήσει το [όριο μεγέθους τοποθεσίας](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) και να διαγράψει το στοιχείο.

- Βεβαιωθείτε ότι δεν έχει γίνει ανάληψη [ελέγχου του στοιχείου](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) σε άλλο χρήστη.

- Τέλος, οι διαχειριστές μπορούν να [χρησιμοποιήσουν SharePoint μοτίβα](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) και πρακτικές (PnP) που περιέχει μια βιβλιοθήκη εντολών του PowerShell που σας επιτρέπουν να εκτελέσετε σύνθετες ενέργειες διαχείρισης, όπως η επιβολή διαγραφής πεισματάρων στοιχείων.
- [Κατάργηση αρχείου PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Κατάργηση φακέλου PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Κατάργηση στοιχείου λίστας PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Κατάργηση λίστας PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Κατάργηση πεδίου PNP (στήλη)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)