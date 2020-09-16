---
title: 2419-δεν είναι δυνατή η ενεργοποίηση-έλεγχος
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
ms.openlocfilehash: 81fd8e33feb2f2b10b04cc7cdc746a8603aa366b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767599"
---
# <a name="unable-to-enable-unified-auditing"></a>Δεν είναι δυνατή η ενεργοποίηση του ενοποιημένου ελέγχου

Όταν προσπαθείτε να ενεργοποιήσετε τον ενοποιημένο έλεγχο για τον οργανισμό σας, ενδέχεται να εμφανιστεί ένα σφάλμα παρόμοιο με το εξής:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Για να επιλύσετε αυτό το πρόβλημα, ακολουθήστε τα παρακάτω βήματα:

1. [Σύνδεση στο Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Εκτελέστε το ακόλουθο cmdlet:

   ```
   Enable-OrganizationCustomization
   ```

3. Περιμένετε 60 λεπτά για να τεθεί σε ισχύ η προηγούμενη ρύθμιση.

4. Εκτελέστε την ακόλουθη εντολή στο Exchange Online PowerShell:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Για περισσότερες πληροφορίες, ανατρέξτε στα ακόλουθα άρθρα:

- [Σύνδεση στο Exchange Online PowerShell με χρήση ελέγχου ταυτότητας πολλών παραγόντων](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Ενεργοποίηση ή απενεργοποίηση της αναζήτησης του αρχείου καταγραφής ελέγχου](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
