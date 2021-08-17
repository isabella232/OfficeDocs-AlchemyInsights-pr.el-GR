---
title: Δικαιώματα ημερολογίου
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: 4bf7680a422f096401f0a87bccd1b8dd11f4489f882bcc06864e37d6a248438c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046104"
---
# <a name="calendar-permissions"></a>Δικαιώματα ημερολογίου

Οι χρήστες μπορούν να αλλάξουν τα δικά τους δικαιώματα ημερολογίου Outlook στο Web ή σε άλλα προγράμματα-πελάτες, αλλά ως διαχειριστής μπορεί να χρειαστεί να διερευνήσετε επίσης.  
Με Exchange cmdlet του PowerShell θα εμφανιστεί το δικαίωμα στο ημερολόγιο ενός χρήστη:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Για να δείτε περισσότερες πληροφορίες, ανατρέξτε στα εξής:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Τα δικαιώματα ημερολογίου χρησιμοποιούνται στην κοινή χρήση ημερολογίων, για να δείτε περισσότερες πληροφορίες σχετικά με την κοινή χρήση Outlook ημερολογίου, ανατρέξτε στα παρακάτω άρθρα:

- [Κοινή χρήση ημερολογίου του Outlook με άλλους](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Κοινή χρήση του ημερολογίου σας στο Outlook στο web για επιχειρήσεις](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Για να αντιμετωπίσετε προβλήματα με τα δικαιώματα ημερολογίου, μπορείτε [να χρησιμοποιήσετε Βοηθός υποστήριξης και αποκατάστασης](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) εργαλείο.