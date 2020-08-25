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
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a>Ο αποστολέας δεν λαμβάνει μηνύματα ηλεκτρονικού ταχυδρομείου που αποστέλλονται στην ομάδα Microsoft 365

Από προεπιλογή, ο αποστολέας ενός μηνύματος ηλεκτρονικού ταχυδρομείου σε μια ομάδα του Microsoft 365 δεν λαμβάνει αντίγραφο του μηνύματος στα Εισερχόμενά του, ακόμα και αν ο αποστολέας είναι μέλος της ομάδας.

Χρησιμοποιήστε αυτήν την εντολή εξω PowerShell για να επιτρέψετε στον αποστολέα να λαμβάνει ένα αντίγραφο κάθε μηνύματος ηλεκτρονικού ταχυδρομείου που αποστέλλει στην ομάδα Microsoft 365:  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

Για να ενεργοποιήσετε τη ρύθμιση για όλα τα γραμματοκιβώτια ταυτόχρονα:

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

**Σημείωση** Οι αλλαγές σε αυτήν τη ρύθμιση θα χρειαστούν έως και μία ώρα για να τεθούν σε ισχύ.