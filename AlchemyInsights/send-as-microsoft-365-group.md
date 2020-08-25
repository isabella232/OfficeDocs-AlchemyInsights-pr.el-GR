---
title: Ομάδα "Αποστολή ως Microsoft 365"
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/19/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: cfb4bd5ce59eeccdd0812d013b8a444aebeb1d4c
ms.sourcegitcommit: 9818d3c8e6b10f23244e51286e2463caf48fffd5
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/21/2020
ms.locfileid: "46871820"
---
# <a name="send-as-microsoft-365-group"></a>Ομάδα "Αποστολή ως Microsoft 365"

Μπορείτε να εκχωρήσετε δικαιώματα αποστολής ως για να επιτρέψετε σε συγκεκριμένους χρήστες να στέλνουν μηνύματα ως ομάδα του Microsoft 365:  

1. Σύνδεση στο Exchange Online PowerShell.  

2. Εκτελέστε την παρακάτω εντολή:  

    Add-RecipientPermission `<GroupName>` -trustee `<MailboxName>` -AccessRights SendAs

Για περισσότερες πληροφορίες, ανατρέξτε στο [θέμα να επιτρέπεται στα μέλη να στέλνουν ως ή να στέλνουν εκ μέρους μιας ομάδας](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).