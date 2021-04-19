---
title: Χρήση του Windows PowerShell για κοινή χρήση πολιτικών και σχέσεων μεταξύ οργανισμών
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 9c52b876160f9577e6cefe7644c29d6fdf3b23fd
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826055"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>Χρήση του Windows PowerShell για κοινή χρήση πολιτικών και σχέσεων μεταξύ οργανισμών


Για τις σχέσεις μεταξύ οργανισμών, εξετάστε τις λεπτομερείς πληροφορίες σύνταξης και παραμέτρων για: [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelation](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  ΚΑΙ  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).

Για να δημιουργήσετε μια πολιτική κοινής χρήσης [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy). Για να  [εφαρμόσετε μια πολιτική κοινής χρήσης σε ένα γραμματοκιβώτιο ή χρήστη](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  πρέπει να χρησιμοποιήσετε έναν συνδυασμό των  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) και [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) με την πολιτική που μόλις δημιουργήσατε. Για να  [τροποποιήσετε, να απενεργοποιήσετε ή να καταργήσετε μια πολιτική κοινής χρήσης](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  πρέπει να χρησιμοποιήσετε το  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) και [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).

**Για να κατανοήσετε πλήρως αυτό το θέμα, διαβάστε:**

[Κοινή χρήση στο Exchange Online](https://docs.microsoft.com/exchange/sharing/sharing)