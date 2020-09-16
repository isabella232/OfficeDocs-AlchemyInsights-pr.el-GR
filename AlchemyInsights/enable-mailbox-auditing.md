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
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="fda18-102">Ενεργοποίηση ελέγχου γραμματοκιβωτίου</span><span class="sxs-lookup"><span data-stu-id="fda18-102">Enable mailbox auditing</span></span>

<span data-ttu-id="fda18-103">Για να ενεργοποιήσετε τον έλεγχο γραμματοκιβωτίου για έναν μεμονωμένο χρήστη ή μια ολόκληρη εταιρεία, τα παρακάτω cmdlet πρέπει να εκτελεστούν από το Remote Power Shell:</span><span class="sxs-lookup"><span data-stu-id="fda18-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="fda18-104">**Μεμονωμένος χρήστης**</span><span class="sxs-lookup"><span data-stu-id="fda18-104">**Single User**</span></span>
  
<span data-ttu-id="fda18-105">Ορίστε-γραμματοκιβώτιο-ταυτότητα "Jane Dow"-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="fda18-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="fda18-106">**Οργάνωση**</span><span class="sxs-lookup"><span data-stu-id="fda18-106">**Organization**</span></span>
  
<span data-ttu-id="fda18-107">Get-Mailbox-ResultSize Unlimited-Filter {RecipientTypeDetails-EQ "UserMailbox"} | Ορίστε-γραμματοκιβώτιο-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="fda18-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="fda18-108">Μάθε περισσότερα</span><span class="sxs-lookup"><span data-stu-id="fda18-108">Learn more</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)
  

