---
title: 2419-unable-to-enable-auditing
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 0566a8d002b1bd9e38f3184824193394e49d56494d347338f96cfcdfdb758f4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007790"
---
# <a name="unable-to-enable-unified-auditing"></a>Δεν είναι δυνατή η ενεργοποίηση του ενοποιημένου ελέγχου

Όταν προσπαθείτε να ενεργοποιήσετε τον ενοποιημένο έλεγχο για τον οργανισμό σας, ενδέχεται να λάβετε ένα σφάλμα παρόμοιο με το εξής:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Για να επιλύσετε αυτό το πρόβλημα, ακολουθήστε τα παρακάτω βήματα:

1. [Σύνδεση να Exchange Online Powershell.](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)

2. Εκτελέστε το ακόλουθο cmdlet:

   ```
   Enable-OrganizationCustomization
   ```

3. Περιμένετε 60 λεπτά για να ισχύει η προηγούμενη ρύθμιση.

4. Εκτελέστε την ακόλουθη εντολή στο Exchange Online PowerShell:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Για πρόσθετες πληροφορίες, ανατρέξτε στα ακόλουθα άρθρα:

- [Σύνδεση να Exchange Online PowerShell χρησιμοποιώντας έλεγχο ταυτότητας πολλών παραγόντων](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Ενεργοποίηση ή απενεργοποίηση της αναζήτησης αρχείου καταγραφής ελέγχου](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
