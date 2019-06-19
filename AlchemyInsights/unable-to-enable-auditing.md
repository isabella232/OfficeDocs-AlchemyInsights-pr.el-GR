---
title: 2419-δεν είναι δυνατή η-σε-Ενεργοποίηση-έλεγχος
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 3af01c03711eed646f0009afb5bea685bc358196
ms.sourcegitcommit: 87153fec6f6468b57893abf4aac073ba4068e67b
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/19/2019
ms.locfileid: "35065645"
---
# <a name="unable-to-enable-unified-auditing"></a><span data-ttu-id="7c058-102">Δεν είναι δυνατή η ενεργοποίηση του ενιαίου ελέγχου</span><span class="sxs-lookup"><span data-stu-id="7c058-102">Unable to enable unified auditing</span></span>

<span data-ttu-id="7c058-103">Κατά την προσπάθειά σας να ενεργοποιήσετε τον ενοποιημένο έλεγχο για τον οργανισμό σας Office 365, ενδέχεται να εμφανιστεί σφάλμα παρόμοιο τα εξής:</span><span class="sxs-lookup"><span data-stu-id="7c058-103">When you try to enable unified auditing for your Office 365 organization, you may receive an error similar the following:</span></span>

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

<span data-ttu-id="7c058-104">Για να επιλύσετε αυτό το ζήτημα, ακολουθήστε τα εξής βήματα:</span><span class="sxs-lookup"><span data-stu-id="7c058-104">To resolve this issue, follow these steps:</span></span>

1. <span data-ttu-id="7c058-105">[Συνδεθείτε με το Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="7c058-105">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="7c058-106">Εκτελέστε την ακόλουθη cmdlet:</span><span class="sxs-lookup"><span data-stu-id="7c058-106">Run the following cmdlet:</span></span>

   ```
   Enable-OrganizationCustomization
   ```

3. <span data-ttu-id="7c058-107">Περιμένετε μέχρι 60 λεπτά για να τεθούν σε ισχύ την προηγούμενη ρύθμιση.</span><span class="sxs-lookup"><span data-stu-id="7c058-107">Wait for 60 minutes for the previous setting to take effect.</span></span>

4. <span data-ttu-id="7c058-108">Εκτελέστε την ακόλουθη εντολή σε PowerShell ηλεκτρονική ανταλλαγή:</span><span class="sxs-lookup"><span data-stu-id="7c058-108">Run the following command in Exchange Online PowerShell:</span></span>

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

<span data-ttu-id="7c058-109">Για περισσότερες πληροφορίες, ανατρέξτε στα ακόλουθα άρθρα:</span><span class="sxs-lookup"><span data-stu-id="7c058-109">For additional information, see the following articles:</span></span>

- [<span data-ttu-id="7c058-110">Συνδεθείτε με το Exchange Online PowerShell χρησιμοποιώντας έλεγχο ταυτότητας πολλών παραγόντων</span><span class="sxs-lookup"><span data-stu-id="7c058-110">Connect to Exchange Online PowerShell using multi-factor authentication</span></span>](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [<span data-ttu-id="7c058-111">Ενεργοποίηση ή απενεργοποίηση της αναζήτησης αρχείου καταγραφής ελέγχου Office 365</span><span class="sxs-lookup"><span data-stu-id="7c058-111">Turn Office 365 audit log search on or off</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off)
