---
title: 929 Κανόνες εισερχομένων για την εκτροπή κανόνων μεταφοράς
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "929"
- "1800021"
ms.assetid: 9733ef4e-db8d-4345-a072-c251480875a1
ms.openlocfilehash: 6b6e64c0332a579e8f6132b08f2f89b15eb4de27
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43724592"
---
# <a name="mail-flow-rules-also-known-as-transport-rules"></a><span data-ttu-id="a08b4-102">Κανόνες ροής αλληλογραφίας (γνωστοί και ως κανόνες μεταφοράς)</span><span class="sxs-lookup"><span data-stu-id="a08b4-102">Mail flow rules (also known as transport rules)</span></span>

- <span data-ttu-id="a08b4-103">Επισκόπηση των κανόνων ροής αλληλογραφίας: [Κανόνες ροής αλληλογραφίας (κανόνες μεταφοράς) στο Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)</span><span class="sxs-lookup"><span data-stu-id="a08b4-103">General overview of mail flow rules: [Mail flow rules (transport rules) in Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)</span></span>

- <span data-ttu-id="a08b4-104">Κανόνες ροής αλληλογραφίας εγκατάστασης: [Διαδικασίες κανόνων ροής αλληλογραφίας στο Exchange Online](https://technet.microsoft.com/library/dn600436.aspx)</span><span class="sxs-lookup"><span data-stu-id="a08b4-104">Setup mail flow rules: [Mail flow rule procedures in Exchange Online](https://technet.microsoft.com/library/dn600436.aspx)</span></span>

- <span data-ttu-id="a08b4-105">Δημιουργία, τροποποίηση και διαγραφή κανόνων ροής αλληλογραφίας: [Διαχείριση κανόνων ροής αλληλογραφίας](https://technet.microsoft.com/library/jj657505.aspx)</span><span class="sxs-lookup"><span data-stu-id="a08b4-105">Create, modify, and delete mail flow rules: [Manage mail flow rules](https://technet.microsoft.com/library/jj657505.aspx)</span></span>

<span data-ttu-id="a08b4-106">Μπορείτε επίσης να διαχειριστείτε κανόνες ροής αλληλογραφίας στο Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="a08b4-106">You can also manage mail flow rules in Exchange Online PowerShell.</span></span> <span data-ttu-id="a08b4-107">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Get-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (προβολή), [Κανόνας νέας μεταφοράς](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (δημιουργία), [Κατάργηση-ΜεταφοράΚανόνας](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (διαγραφή), [Κανόνας set-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (τροποποίηση υπάρχοντος), [Απενεργοποίηση-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (απενεργοποίηση υπάρχοντος) και [Ενεργοποίηση-ΜεταφοράΚανόνας](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (ενεργοποίηση υπάρχοντος).</span><span class="sxs-lookup"><span data-stu-id="a08b4-107">For more information, see [Get-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (view), [New-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (create), [Remove-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (delete), [Set-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (modify existing), [Disable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (disable existing), and [Enable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (enable existing).</span></span>

<span data-ttu-id="a08b4-108">Πρόσθετα cmdlets κανόνα ροής αλληλογραφίας: [Get-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (διαθέσιμες ενέργειες λίστας), [Get-TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (λίστα διαθέσιμες συνθήκες και εξαιρέσεις), [Εξαγωγή-ΜεταφοράRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (κανόνες εξαγωγής) και [Εισαγωγή-ΜεταφοράRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (κανόνες εισαγωγής).</span><span class="sxs-lookup"><span data-stu-id="a08b4-108">Additional mail flow rule cmdlets: [Get-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (list available actions), [Get-TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (list available conditions and exceptions), [Export-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (export rules), and [Import-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (import rules).</span></span>
