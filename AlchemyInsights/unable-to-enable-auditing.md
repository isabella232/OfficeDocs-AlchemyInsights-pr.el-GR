---
title: 2419-ανίκανος-να-ενεργοποίηση-έλεγχος
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 23ad07a6dd943d61d1bd45453089a771cfd51b58
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510428"
---
# <a name="unable-to-enable-unified-auditing"></a><span data-ttu-id="d8090-102">Δεν είναι δυνατή η ενεργοποίηση ενοποιημένου ελέγχου</span><span class="sxs-lookup"><span data-stu-id="d8090-102">Unable to enable unified auditing</span></span>

<span data-ttu-id="d8090-103">Όταν προσπαθείτε να ενεργοποιήσετε τον ενοποιημένο έλεγχο για τον οργανισμό σας, ενδέχεται να λάβετε ένα σφάλμα παρόμοιο με το ακόλουθο:</span><span class="sxs-lookup"><span data-stu-id="d8090-103">When you try to enable unified auditing for your organization, you may receive an error similar the following:</span></span>

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

<span data-ttu-id="d8090-104">Για να επιλύσετε αυτό το ζήτημα, ακολουθήστε τα εξής βήματα:</span><span class="sxs-lookup"><span data-stu-id="d8090-104">To resolve this issue, follow these steps:</span></span>

1. <span data-ttu-id="d8090-105">[Σύνδεση στο Ηλεκτρονικό Powershell του Exchange](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="d8090-105">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="d8090-106">Εκτελέστε το ακόλουθο cmdlet:</span><span class="sxs-lookup"><span data-stu-id="d8090-106">Run the following cmdlet:</span></span>

   ```
   Enable-OrganizationCustomization
   ```

3. <span data-ttu-id="d8090-107">Περιμένετε 60 λεπτά για να τεθεί σε ισχύ η προηγούμενη ρύθμιση.</span><span class="sxs-lookup"><span data-stu-id="d8090-107">Wait for 60 minutes for the previous setting to take effect.</span></span>

4. <span data-ttu-id="d8090-108">Εκτελέστε την ακόλουθη εντολή στο Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="d8090-108">Run the following command in Exchange Online PowerShell:</span></span>

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

<span data-ttu-id="d8090-109">Για περισσότερες πληροφορίες, ανατρέξτε στα ακόλουθα άρθρα:</span><span class="sxs-lookup"><span data-stu-id="d8090-109">For additional information, see the following articles:</span></span>

- [<span data-ttu-id="d8090-110">Σύνδεση στο Exchange Online PowerShell με χρήση ελέγχου ταυτότητας πολλών παραγόντων</span><span class="sxs-lookup"><span data-stu-id="d8090-110">Connect to Exchange Online PowerShell using multi-factor authentication</span></span>](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [<span data-ttu-id="d8090-111">Ενεργοποίηση ή απενεργοποίηση της αναζήτησης καταγραφής ελέγχου</span><span class="sxs-lookup"><span data-stu-id="d8090-111">Turn audit log search on or off</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
