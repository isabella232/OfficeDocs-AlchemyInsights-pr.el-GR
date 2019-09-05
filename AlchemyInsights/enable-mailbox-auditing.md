---
title: Ενεργοποίηση ελέγχου γραμματοκιβωτίου
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 73517f46935a67a4a8a3e4770090ac897fe67979
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736253"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="c8ada-102">Ενεργοποίηση ελέγχου γραμματοκιβωτίου</span><span class="sxs-lookup"><span data-stu-id="c8ada-102">Enable mailbox auditing</span></span>

<span data-ttu-id="c8ada-103">Για να ενεργοποιήσετε τον έλεγχο γραμματοκιβωτίου για έναν μεμονωμένο χρήστη ή για έναν ολόκληρο οργανισμό, τα ακόλουθα cmdlet πρέπει να εκτελούνται από το κέλυφος απομακρυσμένης ισχύος:</span><span class="sxs-lookup"><span data-stu-id="c8ada-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="c8ada-104">**Ένας χρήστης**</span><span class="sxs-lookup"><span data-stu-id="c8ada-104">**Single User**</span></span>
  
<span data-ttu-id="c8ada-105">Set-γραμματοκιβώτιο-ταυτότητα "Τζέιν Ντάου"-ελεγμένα $true</span><span class="sxs-lookup"><span data-stu-id="c8ada-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="c8ada-106">**Οργάνωση**</span><span class="sxs-lookup"><span data-stu-id="c8ada-106">**Organization**</span></span>
  
<span data-ttu-id="c8ada-107">Αποκτήστε-γραμματοκιβώτιο-αποτελέσμα απεριόριστου-φίλτρο {συνταγές Σετ-γραμματοκιβώτιο-ελεγμένα $true</span><span class="sxs-lookup"><span data-stu-id="c8ada-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="c8ada-108">Μάθε περισσότερα</span><span class="sxs-lookup"><span data-stu-id="c8ada-108">Learn more</span></span>](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

