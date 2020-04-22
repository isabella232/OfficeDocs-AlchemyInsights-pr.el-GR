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
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="8ede4-102">Ενεργοποίηση ελέγχου γραμματοκιβωτίου</span><span class="sxs-lookup"><span data-stu-id="8ede4-102">Enable mailbox auditing</span></span>

<span data-ttu-id="8ede4-103">Για να ενεργοποιήσετε τον έλεγχο γραμματοκιβωτίου για έναν μεμονωμένο χρήστη ή για έναν ολόκληρο οργανισμό, τα ακόλουθα cmdlets πρέπει να εκτελούνται από το απομακρυσμένο κέλυφος ενέργειας:</span><span class="sxs-lookup"><span data-stu-id="8ede4-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="8ede4-104">**Μεμονωμένος χρήστης**</span><span class="sxs-lookup"><span data-stu-id="8ede4-104">**Single User**</span></span>
  
<span data-ttu-id="8ede4-105">Set-Γραμματοκιβώτιο -Ταυτότητα "Jane Dow" -ΈλεγχοςΕνεργοποιημένο $true</span><span class="sxs-lookup"><span data-stu-id="8ede4-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="8ede4-106">**Οργάνωση**</span><span class="sxs-lookup"><span data-stu-id="8ede4-106">**Organization**</span></span>
  
<span data-ttu-id="8ede4-107">Get-Γραμματοκιβώτιο -ResultSize Απεριόριστα -Φίλτρο {RecipientTypeDetails -eq "UserMailbox"} | Ορισμός γραμματοκιβωτίου -Ενεργοποίηση ελέγχου $true</span><span class="sxs-lookup"><span data-stu-id="8ede4-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="8ede4-108">Μάθε περισσότερα</span><span class="sxs-lookup"><span data-stu-id="8ede4-108">Learn more</span></span>](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

