---
title: 929 κανόνες για τα εισερχόμενα deflectTransport κανόνες
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/15/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9733ef4e-db8d-4345-a072-c251480875a1
ms.openlocfilehash: 45c542191dd5ef67cef464e1f204358471c21948
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29928584"
---
# <a name="mail-flow-rules-also-known-as-transport-rules"></a><span data-ttu-id="98523-102">Κανόνες ροής αλληλογραφίας (γνωστό και ως κανόνες μεταφοράς)</span><span class="sxs-lookup"><span data-stu-id="98523-102">Mail flow rules (also known as transport rules)</span></span>

- <span data-ttu-id="98523-103">Γενική επισκόπηση των κανόνων ροής αλληλογραφίας: [αλληλογραφίας ροή κανόνες (κανόνες μεταφοράς) στο Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)</span><span class="sxs-lookup"><span data-stu-id="98523-103">General overview of mail flow rules: [Mail flow rules (transport rules) in Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)</span></span>
    
- <span data-ttu-id="98523-104">Ρύθμιση κανόνων ροής αλληλογραφίας: [αλληλογραφίας ροή διαδικασίες κανόνα στο Exchange Online](https://technet.microsoft.com/library/dn600436.aspx)</span><span class="sxs-lookup"><span data-stu-id="98523-104">Setup mail flow rules: [Mail flow rule procedures in Exchange Online](https://technet.microsoft.com/library/dn600436.aspx)</span></span>
    
- <span data-ttu-id="98523-105">Δημιουργία, τροποποίηση και διαγραφή κανόνων ροής αλληλογραφίας: [Διαχείριση κανόνων ροής αλληλογραφίας](https://technet.microsoft.com/library/jj657505.aspx)</span><span class="sxs-lookup"><span data-stu-id="98523-105">Create, modify, and delete mail flow rules: [Manage mail flow rules](https://technet.microsoft.com/library/jj657505.aspx)</span></span>
    
<span data-ttu-id="98523-p101">Μπορείτε επίσης να διαχειριστείτε κανόνες ροής αλληλογραφίας στον Exchange Online PowerShell. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Get-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (προβολή), [Δημιουργία TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (δημιουργία), [Κατάργηση TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (διαγραφή), το [Σύνολο TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (τροποποίηση υπαρχόντων), [TransportRule απενεργοποίηση](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (disable υπάρχον), και [Ενεργοποίηση TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (ενεργοποιήσετε το ήδη υπάρχον).</span><span class="sxs-lookup"><span data-stu-id="98523-p101">You can also manage mail flow rules in Exchange Online PowerShell. For more information, see [Get-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (view), [New-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (create), [Remove-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (delete), [Set-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (modify existing), [Disable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (disable existing), and [Enable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (enable existing).</span></span> 
  
<span data-ttu-id="98523-108">Cmdlets κανόνα ροής πρόσθετες αλληλογραφίας: [Get-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (λίστα διαθέσιμες ενέργειες), [Get-TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (λίστα διαθέσιμες συνθήκες και εξαιρέσεις), [TransportRuleCollection εξαγωγής](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (εξαγωγή κανόνων) και [ Εισαγωγή TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (εισαγωγή κανόνων).</span><span class="sxs-lookup"><span data-stu-id="98523-108">Additional mail flow rule cmdlets: [Get-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (list available actions), [Get-TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (list available conditions and exceptions), [Export-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (export rules), and [Import-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (import rules).</span></span> 
  

