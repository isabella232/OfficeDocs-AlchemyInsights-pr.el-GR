---
title: Ενεργοποίηση ελέγχου γραμματοκιβωτίου
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: ae11d6be0789a5662d202b85268480a3d42922c4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703571"
---
# <a name="enable-mailbox-auditing"></a>Ενεργοποίηση ελέγχου γραμματοκιβωτίου

Για να ενεργοποιήσετε τον έλεγχο γραμματοκιβωτίου για έναν μεμονωμένο χρήστη ή για έναν ολόκληρο οργανισμό, τα ακόλουθα cmdlets πρέπει να εκτελούνται από το απομακρυσμένο κέλυφος ενέργειας:
  
 **Μεμονωμένος χρήστης**
  
Set-Γραμματοκιβώτιο -Ταυτότητα "Jane Dow" -ΈλεγχοςΕνεργοποιημένο $true
  
 **Οργάνωση**
  
Get-Γραμματοκιβώτιο -ResultSize Απεριόριστα -Φίλτρο {RecipientTypeDetails -eq "UserMailbox"} | Ορισμός γραμματοκιβωτίου -Ενεργοποίηση ελέγχου $true
  
[Μάθε περισσότερα](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

