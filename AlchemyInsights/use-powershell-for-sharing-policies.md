---
title: Χρήση πολιτικών και σχέσεων οργανισμού του PowerShell για κοινή χρήση
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 717cdd6827e243ac6bf375209a911937c97088d2
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862086"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>Χρήση πολιτικών και σχέσεων οργανισμού του PowerShell για κοινή χρήση


Για σχέσεις οργανισμού, ανατρέξτε στις λεπτομερείς πληροφορίες σύνταξης και παραμέτρων για : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship) ΚΑΙ [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).

Για να δημιουργήσετε πολιτική κοινής χρήσης, χρησιμοποιήστε [την Πολιτική νέας κατανομής](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy). Για να [εφαρμόσετε μια πολιτική κοινής χρήσης σε ένα γραμματοκιβώτιο ή χρήστη,](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes) πρέπει να χρησιμοποιήσετε ένα συνδυασμό [set-mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) και [get-mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) με τη νέα πολιτική. Για να [τροποποιήσετε, να απενεργοποιήσετε ή να καταργήσετε μια πολιτική κοινής χρήσης,](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy) πρέπει να χρησιμοποιήσετε την [Πολιτική κοινής χρήσης και](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) την πολιτική [κατάργησης κοινής χρήσης](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).

**Για την πλήρη κατανόηση αυτού του θέματος παρακαλούμε διαβάστε:**

[Κοινή χρήση στο Exchange Online](https://docs.microsoft.com/exchange/sharing/sharing)