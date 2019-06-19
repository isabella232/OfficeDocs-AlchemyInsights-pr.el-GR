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
# <a name="unable-to-enable-unified-auditing"></a>Δεν είναι δυνατή η ενεργοποίηση του ενιαίου ελέγχου

Κατά την προσπάθειά σας να ενεργοποιήσετε τον ενοποιημένο έλεγχο για τον οργανισμό σας Office 365, ενδέχεται να εμφανιστεί σφάλμα παρόμοιο τα εξής:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Για να επιλύσετε αυτό το ζήτημα, ακολουθήστε τα εξής βήματα:

1. [Συνδεθείτε με το Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Εκτελέστε την ακόλουθη cmdlet:

   ```
   Enable-OrganizationCustomization
   ```

3. Περιμένετε μέχρι 60 λεπτά για να τεθούν σε ισχύ την προηγούμενη ρύθμιση.

4. Εκτελέστε την ακόλουθη εντολή σε PowerShell ηλεκτρονική ανταλλαγή:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Για περισσότερες πληροφορίες, ανατρέξτε στα ακόλουθα άρθρα:

- [Συνδεθείτε με το Exchange Online PowerShell χρησιμοποιώντας έλεγχο ταυτότητας πολλών παραγόντων](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Ενεργοποίηση ή απενεργοποίηση της αναζήτησης αρχείου καταγραφής ελέγχου Office 365](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off)
