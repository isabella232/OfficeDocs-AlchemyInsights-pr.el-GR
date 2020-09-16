---
title: Δικαιώματα ημερολογίου
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: cfee520e26587c0a649c08084853c31232d027f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748793"
---
# <a name="calendar-permissions"></a>Δικαιώματα ημερολογίου

Οι χρήστες μπορούν να αλλάξουν τα δικά τους δικαιώματα ημερολογίου με το Outlook στο Web ή σε άλλα προγράμματα-πελάτες, αλλά ως διαχειριστής μπορεί να χρειαστεί να ερευνήσετε επίσης.  
Με το cmdlet του Exchange PowerShell θα σας εμφανίσει το δικαίωμα στο ημερολόγιο ενός χρήστη:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Για να δείτε περισσότερες πληροφορίες, ανατρέξτε στα παρακάτω θέματα:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Ορίστε-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Τα δικαιώματα ημερολογίου χρησιμοποιούνται στην κοινή χρήση ημερολογίων, για να δείτε περισσότερες πληροφορίες σχετικά με την κοινή χρήση ενός ημερολογίου του Outlook, ανατρέξτε σε αυτά τα άρθρα:

- [Κοινή χρήση ημερολογίου του Outlook με άλλους](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Κοινή χρήση του ημερολογίου σας στο Outlook στο Web για επαγγελματικούς λόγους](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Για την αντιμετώπιση των δικαιωμάτων ημερολογίου, μπορείτε να χρησιμοποιήσετε το εργαλείο [υποστήριξης και αποκατάστασης του βοηθού](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) .