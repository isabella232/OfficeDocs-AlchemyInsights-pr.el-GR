---
title: Ο αποστολέας δεν λαμβάνει μηνύματα ηλεκτρονικού ταχυδρομείου που αποστέλλονται στην ομάδα Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: b3b438e17c35f18289d3e9c3ca89d16a6f2a065f
ms.sourcegitcommit: dcca0df53f9194f406cf3a5f6b046cb33a0a5b03
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/21/2020
ms.locfileid: "46871818"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a><span data-ttu-id="15f79-102">Ο αποστολέας δεν λαμβάνει μηνύματα ηλεκτρονικού ταχυδρομείου που αποστέλλονται στην ομάδα Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="15f79-102">Sender does not receive email sent to Microsoft 365 group</span></span>

<span data-ttu-id="15f79-103">Από προεπιλογή, ο αποστολέας ενός μηνύματος ηλεκτρονικού ταχυδρομείου σε μια ομάδα του Microsoft 365 δεν λαμβάνει αντίγραφο του μηνύματος στα Εισερχόμενά του, ακόμα και αν ο αποστολέας είναι μέλος της ομάδας.</span><span class="sxs-lookup"><span data-stu-id="15f79-103">By default, the sender of an email message to a Microsoft 365 group doesn't receive a copy of the message in their Inbox, even if the sender is a member of the group.</span></span>

<span data-ttu-id="15f79-104">Χρησιμοποιήστε αυτήν την εντολή εξω PowerShell για να επιτρέψετε στον αποστολέα να λαμβάνει ένα αντίγραφο κάθε μηνύματος ηλεκτρονικού ταχυδρομείου που αποστέλλει στην ομάδα Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="15f79-104">Use this EXO PowerShell command to allow the sender to receive a copy of each email they send to the Microsoft 365 group:</span></span>  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

<span data-ttu-id="15f79-105">Για να ενεργοποιήσετε τη ρύθμιση για όλα τα γραμματοκιβώτια ταυτόχρονα:</span><span class="sxs-lookup"><span data-stu-id="15f79-105">To enable the setting for all mailboxes at once:</span></span>

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

<span data-ttu-id="15f79-106">**Σημείωση** Οι αλλαγές σε αυτήν τη ρύθμιση θα χρειαστούν έως και μία ώρα για να τεθούν σε ισχύ.</span><span class="sxs-lookup"><span data-stu-id="15f79-106">**Note** Changes to this setting take up to an hour to take effect.</span></span>