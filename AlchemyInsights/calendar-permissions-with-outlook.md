---
title: Δικαιώματα ημερολογίου
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: 78f27014c60badc801212177dd455ef2a0de5a9e
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862095"
---
# <a name="calendar-permissions"></a>Δικαιώματα ημερολογίου

Οι χρήστες μπορούν να αλλάξουν τα δικά τους δικαιώματα ημερολογίου με το Outlook στο Web ή σε άλλους υπολογιστές-πελάτες, αλλά ως διαχειριστής ίσως χρειαστεί να εξετάσετε επίσης.  
Με το cmdlet Exchange PowerShell θα σας δείξει το δικαίωμα στο ημερολόγιο ενός χρήστη:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Για να δείτε περισσότερες πληροφορίες, ανατρέξτε στα εξής:

- [Λήψη γραμματοκιβωτίουΑδιάπλωτάπτυξη](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Ορισμός γραμματοκιβωτίουΑποστολής](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Αριθμός δικαιωματικών φακέλων γραμματοκιβωτίου](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Τα δικαιώματα ημερολογίου χρησιμοποιούνται στην κοινή χρήση ημερολογίων, για να δείτε περισσότερες πληροφορίες σχετικά με την κοινή χρήση ενός ημερολογίου του Outlook, ανατρέξτε στα εξής άρθρα:

- [Κοινή χρήση ημερολογίου του Outlook με άλλους](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Κοινή χρήση του ημερολογίου σας στο Outlook στο web για επιχειρήσεις](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Για να αντιμετωπίσετε προβλήματα με τα δικαιώματα ημερολογίου, μπορείτε να χρησιμοποιήσετε το εργαλείο [Βοηθού υποστήριξης και αποκατάστασης.](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f)