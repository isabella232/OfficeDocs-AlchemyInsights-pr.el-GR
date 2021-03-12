---
title: Χρήση του Windows PowerShell για κοινή χρήση πολιτικών και σχέσεων μεταξύ οργανισμών
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: cd1d34e4dae474e61c799ca9234b2f18c718f27b
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709466"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a><span data-ttu-id="a59fc-102">Χρήση του Windows PowerShell για κοινή χρήση πολιτικών και σχέσεων μεταξύ οργανισμών</span><span class="sxs-lookup"><span data-stu-id="a59fc-102">Use PowerShell for Sharing policies and Organization relationships</span></span>


<span data-ttu-id="a59fc-103">Για τις σχέσεις μεταξύ οργανισμών, εξετάστε τις λεπτομερείς πληροφορίες σύνταξης και παραμέτρων για: [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelation](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  ΚΑΙ  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span><span class="sxs-lookup"><span data-stu-id="a59fc-103">For Organization relationships please review the detailed syntax and parameter information for : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  AND  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span></span>

<span data-ttu-id="a59fc-104">Για να δημιουργήσετε μια πολιτική κοινής χρήσης [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span><span class="sxs-lookup"><span data-stu-id="a59fc-104">To create sharing policy use [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span></span> <span data-ttu-id="a59fc-105">Για να  [εφαρμόσετε μια πολιτική κοινής χρήσης σε ένα γραμματοκιβώτιο ή χρήστη](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  πρέπει να χρησιμοποιήσετε έναν συνδυασμό των  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) και [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) με την πολιτική που μόλις δημιουργήσατε.</span><span class="sxs-lookup"><span data-stu-id="a59fc-105">To  [apply a sharing policy to a mailbox or user](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  you need to use a combination of  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) and [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) with the newly created policy.</span></span> <span data-ttu-id="a59fc-106">Για να  [τροποποιήσετε, να απενεργοποιήσετε ή να καταργήσετε μια πολιτική κοινής χρήσης](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  πρέπει να χρησιμοποιήσετε το  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) και [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span><span class="sxs-lookup"><span data-stu-id="a59fc-106">To  [modify, disable or remove a sharing policy](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  you need to use  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) and [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span></span>

<span data-ttu-id="a59fc-107">**Για να κατανοήσετε πλήρως αυτό το θέμα, διαβάστε:**</span><span class="sxs-lookup"><span data-stu-id="a59fc-107">**For full understanding of this topic please read:**</span></span>

[<span data-ttu-id="a59fc-108">Κοινή χρήση στο Exchange Online</span><span class="sxs-lookup"><span data-stu-id="a59fc-108">Sharing in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing)