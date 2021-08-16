---
title: Ενεργοποίηση ελέγχου γραμματοκιβωτίου
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 176fdc57c6453cafe6ca773d845f8f59ea782089e3e33ad70909ed495aa1a8c4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54003020"
---
# <a name="enable-mailbox-auditing"></a>Ενεργοποίηση ελέγχου γραμματοκιβωτίου

Για να ενεργοποιήσετε τον έλεγχο γραμματοκιβωτίου είτε για έναν μεμονωμένο χρήστη είτε για έναν ολόκληρο οργανισμό, πρέπει να εκτελούνται τα ακόλουθα cmdlet από το Απομακρυσμένο Power Shell:
  
 **Μεμονωμένος χρήστης**
  
Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true
  
 **Οργανισμός**
  
Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true
  
[Μάθετε περισσότερα](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)
  

