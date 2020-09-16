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
# <a name="calendar-permissions"></a><span data-ttu-id="c9c85-102">Δικαιώματα ημερολογίου</span><span class="sxs-lookup"><span data-stu-id="c9c85-102">Calendar Permissions</span></span>

<span data-ttu-id="c9c85-103">Οι χρήστες μπορούν να αλλάξουν τα δικά τους δικαιώματα ημερολογίου με το Outlook στο Web ή σε άλλα προγράμματα-πελάτες, αλλά ως διαχειριστής μπορεί να χρειαστεί να ερευνήσετε επίσης.</span><span class="sxs-lookup"><span data-stu-id="c9c85-103">Users can change their own Calendar Permissions with Outlook on the Web or other clients, but as an admin you may need to investigate as well.</span></span>  
<span data-ttu-id="c9c85-104">Με το cmdlet του Exchange PowerShell θα σας εμφανίσει το δικαίωμα στο ημερολόγιο ενός χρήστη:</span><span class="sxs-lookup"><span data-stu-id="c9c85-104">With Exchange PowerShell cmdlet will show you the permission on a user’s calendar:</span></span>

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

<span data-ttu-id="c9c85-105">Για να δείτε περισσότερες πληροφορίες, ανατρέξτε στα παρακάτω θέματα:</span><span class="sxs-lookup"><span data-stu-id="c9c85-105">To see more information see the following:</span></span>

- [<span data-ttu-id="c9c85-106">Get-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="c9c85-106">Get-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="c9c85-107">Ορίστε-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="c9c85-107">Set-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="c9c85-108">Add-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="c9c85-108">Add-MailboxFolderPermission</span></span>](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

<span data-ttu-id="c9c85-109">Τα δικαιώματα ημερολογίου χρησιμοποιούνται στην κοινή χρήση ημερολογίων, για να δείτε περισσότερες πληροφορίες σχετικά με την κοινή χρήση ενός ημερολογίου του Outlook, ανατρέξτε σε αυτά τα άρθρα:</span><span class="sxs-lookup"><span data-stu-id="c9c85-109">Calendar Permissions are used in the sharing of calendars, to see more information about sharing an Outlook calendar, see these articles:</span></span>

- [<span data-ttu-id="c9c85-110">Κοινή χρήση ημερολογίου του Outlook με άλλους</span><span class="sxs-lookup"><span data-stu-id="c9c85-110">Share an Outlook calendar with other people</span></span>](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [<span data-ttu-id="c9c85-111">Κοινή χρήση του ημερολογίου σας στο Outlook στο Web για επαγγελματικούς λόγους</span><span class="sxs-lookup"><span data-stu-id="c9c85-111">Share your calendar in Outlook on the web for business</span></span>](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

<span data-ttu-id="c9c85-112">Για την αντιμετώπιση των δικαιωμάτων ημερολογίου, μπορείτε να χρησιμοποιήσετε το εργαλείο [υποστήριξης και αποκατάστασης του βοηθού](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) .</span><span class="sxs-lookup"><span data-stu-id="c9c85-112">To troubleshoot Calendar Permission you can use the [Support and Recovery Assistant](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) tool.</span></span>