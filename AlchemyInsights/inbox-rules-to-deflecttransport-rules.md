---
title: κανόνες εισερχομένων του 929 σε κανόνες deflectTransport
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "929"
- "1800021"
ms.assetid: 9733ef4e-db8d-4345-a072-c251480875a1
ms.openlocfilehash: abb729c40fb87bcca8cc03c95aa4677597d20c08
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47778691"
---
# <a name="mail-flow-rules-also-known-as-transport-rules"></a><span data-ttu-id="6c1cb-102">Κανόνες ροής αλληλογραφίας (γνωστοί και ως κανόνες μεταφοράς)</span><span class="sxs-lookup"><span data-stu-id="6c1cb-102">Mail flow rules (also known as transport rules)</span></span>

- <span data-ttu-id="6c1cb-103">Γενική επισκόπηση των κανόνων ροής αλληλογραφίας: [κανόνες ροής αλληλογραφίας (κανόνες μεταφοράς) στο Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)</span><span class="sxs-lookup"><span data-stu-id="6c1cb-103">General overview of mail flow rules: [Mail flow rules (transport rules) in Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)</span></span>

- <span data-ttu-id="6c1cb-104">Κανόνες ροής αλληλογραφίας εγκατάστασης: [διαδικασίες κανόνα ροής αλληλογραφίας στο Exchange Online](https://technet.microsoft.com/library/dn600436.aspx)</span><span class="sxs-lookup"><span data-stu-id="6c1cb-104">Setup mail flow rules: [Mail flow rule procedures in Exchange Online](https://technet.microsoft.com/library/dn600436.aspx)</span></span>

- <span data-ttu-id="6c1cb-105">Δημιουργία, τροποποίηση και διαγραφή κανόνων ροής αλληλογραφίας: [Διαχείριση κανόνων ροής αλληλογραφίας](https://technet.microsoft.com/library/jj657505.aspx)</span><span class="sxs-lookup"><span data-stu-id="6c1cb-105">Create, modify, and delete mail flow rules: [Manage mail flow rules](https://technet.microsoft.com/library/jj657505.aspx)</span></span>

<span data-ttu-id="6c1cb-106">Μπορείτε επίσης να διαχειριστείτε κανόνες ροής αλληλογραφίας στο Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="6c1cb-106">You can also manage mail flow rules in Exchange Online PowerShell.</span></span> <span data-ttu-id="6c1cb-107">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Get-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (View), [New-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (Create), [Remove-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (Delete), [TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (Modify υπάρχοντα), [disable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (απενεργοποίηση υπάρχουσας) και [Enable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (Ενεργοποίηση υπάρχοντος).</span><span class="sxs-lookup"><span data-stu-id="6c1cb-107">For more information, see [Get-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (view), [New-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (create), [Remove-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (delete), [Set-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (modify existing), [Disable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (disable existing), and [Enable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (enable existing).</span></span>

<span data-ttu-id="6c1cb-108">Πρόσθετα cmdlet κανόνα ροής αλληλογραφίας: [Get-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (λίστα διαθέσιμες ενέργειες), [Get-TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (λίστα διαθέσιμων συνθηκών και εξαιρέσεων), [εξαγωγή-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (κανόνες εξαγωγής) και [Import-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (κανόνες εισαγωγής).</span><span class="sxs-lookup"><span data-stu-id="6c1cb-108">Additional mail flow rule cmdlets: [Get-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (list available actions), [Get-TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (list available conditions and exceptions), [Export-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (export rules), and [Import-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (import rules).</span></span>
