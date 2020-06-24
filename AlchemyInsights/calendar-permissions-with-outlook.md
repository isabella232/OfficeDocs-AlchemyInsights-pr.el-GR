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
# <a name="calendar-permissions"></a><span data-ttu-id="2f939-102">Δικαιώματα ημερολογίου</span><span class="sxs-lookup"><span data-stu-id="2f939-102">Calendar Permissions</span></span>

<span data-ttu-id="2f939-103">Οι χρήστες μπορούν να αλλάξουν τα δικά τους δικαιώματα ημερολογίου με το Outlook στο Web ή σε άλλους υπολογιστές-πελάτες, αλλά ως διαχειριστής ίσως χρειαστεί να εξετάσετε επίσης.</span><span class="sxs-lookup"><span data-stu-id="2f939-103">Users can change their own Calendar Permissions with Outlook on the Web or other clients, but as an admin you may need to investigate as well.</span></span>  
<span data-ttu-id="2f939-104">Με το cmdlet Exchange PowerShell θα σας δείξει το δικαίωμα στο ημερολόγιο ενός χρήστη:</span><span class="sxs-lookup"><span data-stu-id="2f939-104">With Exchange PowerShell cmdlet will show you the permission on a user’s calendar:</span></span>

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

<span data-ttu-id="2f939-105">Για να δείτε περισσότερες πληροφορίες, ανατρέξτε στα εξής:</span><span class="sxs-lookup"><span data-stu-id="2f939-105">To see more information see the following:</span></span>

- [<span data-ttu-id="2f939-106">Λήψη γραμματοκιβωτίουΑδιάπλωτάπτυξη</span><span class="sxs-lookup"><span data-stu-id="2f939-106">Get-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="2f939-107">Ορισμός γραμματοκιβωτίουΑποστολής</span><span class="sxs-lookup"><span data-stu-id="2f939-107">Set-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="2f939-108">Αριθμός δικαιωματικών φακέλων γραμματοκιβωτίου</span><span class="sxs-lookup"><span data-stu-id="2f939-108">Add-MailboxFolderPermission</span></span>](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

<span data-ttu-id="2f939-109">Τα δικαιώματα ημερολογίου χρησιμοποιούνται στην κοινή χρήση ημερολογίων, για να δείτε περισσότερες πληροφορίες σχετικά με την κοινή χρήση ενός ημερολογίου του Outlook, ανατρέξτε στα εξής άρθρα:</span><span class="sxs-lookup"><span data-stu-id="2f939-109">Calendar Permissions are used in the sharing of calendars, to see more information about sharing an Outlook calendar, see these articles:</span></span>

- [<span data-ttu-id="2f939-110">Κοινή χρήση ημερολογίου του Outlook με άλλους</span><span class="sxs-lookup"><span data-stu-id="2f939-110">Share an Outlook calendar with other people</span></span>](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [<span data-ttu-id="2f939-111">Κοινή χρήση του ημερολογίου σας στο Outlook στο web για επιχειρήσεις</span><span class="sxs-lookup"><span data-stu-id="2f939-111">Share your calendar in Outlook on the web for business</span></span>](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

<span data-ttu-id="2f939-112">Για να αντιμετωπίσετε προβλήματα με τα δικαιώματα ημερολογίου, μπορείτε να χρησιμοποιήσετε το εργαλείο [Βοηθού υποστήριξης και αποκατάστασης.](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f)</span><span class="sxs-lookup"><span data-stu-id="2f939-112">To troubleshoot Calendar Permission you can use the [Support and Recovery Assistant](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) tool.</span></span>