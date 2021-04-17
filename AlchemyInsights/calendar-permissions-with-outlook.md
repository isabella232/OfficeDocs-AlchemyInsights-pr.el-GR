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
ms.openlocfilehash: bbd49134bd4a4451649b76bb5f60b19065910cae
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819908"
---
# <a name="calendar-permissions"></a>Δικαιώματα ημερολογίου

Οι χρήστες μπορούν να αλλάξουν τα δικά τους δικαιώματα ημερολογίου με το Outlook στο Web ή άλλα προγράμματα-πελάτες, αλλά ως διαχειριστής ίσως χρειαστεί να διερευνήσετε επίσης.  
Με το cmdlet του Exchange PowerShell θα εμφανιστεί το δικαίωμα στο ημερολόγιο ενός χρήστη:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Για να δείτε περισσότερες πληροφορίες, ανατρέξτε στα εξής:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Τα δικαιώματα ημερολογίου χρησιμοποιούνται στην κοινή χρήση ημερολογίων, για να δείτε περισσότερες πληροφορίες σχετικά με την κοινή χρήση ενός ημερολογίου του Outlook, ανατρέξτε στα παρακάτω άρθρα:

- [Κοινή χρήση ημερολογίου του Outlook με άλλους](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Κοινή χρήση του ημερολογίου σας στο Outlook στο web για επιχειρήσεις](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Για να αντιμετωπίσετε προβλήματα με τα δικαιώματα ημερολογίου, μπορείτε [να χρησιμοποιήσετε το εργαλείο "Βοηθός υποστήριξης και αποκατάστασης".](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f)