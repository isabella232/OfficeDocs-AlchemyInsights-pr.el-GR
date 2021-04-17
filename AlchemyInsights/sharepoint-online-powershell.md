---
title: Sharepoint Online PowerShell
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 839a70282b4dd619e9dbe8167ef0e409e468b1ad
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830582"
---
# <a name="sharepoint-online-powershell"></a>Sharepoint Online PowerShell

Εργάζεστε με το PowerShell ή δέσμες ενεργειών μέσα στο Sharepoint Online; Για περισσότερες πληροφορίες, επισκεφθείτε τις παρακάτω συνδέσεις.
- [Γρήγορα αποτελέσματα με το Κέλυφος διαχείρισης του SharePoint Online](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [Σύνδεση στο SPO PowerShell με έλεγχο ταυτότητας πολλών παραγόντων (MFA)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- [Τα μοτίβα και οι πρακτικές του SharePoint (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) περιέχουν μια βιβλιοθήκη εντολών του PowerShell που σας επιτρέπει να εκτελείτε σύνθετες ενέργειες διαχείρισης προς το SPO.

> [!NOTE]
> - Εάν αντιμετωπίζετε προβλήματα σύνδεσης με το κέλυφος διαχείρισης SPO, βεβαιωθείτε ότι έχετε [](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) ενημερώσει την πιο πρόσφατη έκδοση και προσπαθήστε να εισαγάγετε ξανά τη λειτουργική μονάδα χρησιμοποιώντας *τη "Εισαγωγή λειτουργικής μονάδας Microsoft.Online.SharePoint.PowerShell".*
> - Εάν προσπαθείτε να εκτελέσετε δέσμες ενεργειών μοντέλου αντικειμένου από την πλευρά του προγράμματος-πελάτη, θα πρέπει να έχετε εγκαταστήσει το SDK στοιχείων προγράμματος-πελάτη του [Sharepoint Online](https://www.microsoft.com/download/details.aspx?id=42038) στον τοπικό υπολογιστή σας.
> - Εάν αντιμετωπίζετε προβλήματα κατά την εκτέλεση δεσμών ενεργειών από το PowerShell, μπορείτε να εξετάσετε το ενδεχόμενο να εκτελείτε το PowerShell ως διαχειριστής και να αλλάξετε την [πολιτική εκτέλεσης.](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)