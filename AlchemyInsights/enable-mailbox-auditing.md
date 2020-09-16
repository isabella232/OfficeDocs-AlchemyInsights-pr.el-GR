---
title: Ενεργοποίηση ελέγχου γραμματοκιβωτίου
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 404ef9ecd824541f98471bb8797f5f6e025012b7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806291"
---
# <a name="enable-mailbox-auditing"></a>Ενεργοποίηση ελέγχου γραμματοκιβωτίου

Για να ενεργοποιήσετε τον έλεγχο γραμματοκιβωτίου για έναν μεμονωμένο χρήστη ή μια ολόκληρη εταιρεία, τα παρακάτω cmdlet πρέπει να εκτελεστούν από το Remote Power Shell:
  
 **Μεμονωμένος χρήστης**
  
Ορίστε-γραμματοκιβώτιο-ταυτότητα "Jane Dow"-AuditEnabled $true
  
 **Οργάνωση**
  
Get-Mailbox-ResultSize Unlimited-Filter {RecipientTypeDetails-EQ "UserMailbox"} | Ορίστε-γραμματοκιβώτιο-AuditEnabled $true
  
[Μάθε περισσότερα](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)
  

