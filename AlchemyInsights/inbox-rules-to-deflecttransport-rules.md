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
# <a name="mail-flow-rules-also-known-as-transport-rules"></a>Κανόνες ροής αλληλογραφίας (γνωστοί και ως κανόνες μεταφοράς)

- Γενική επισκόπηση των κανόνων ροής αλληλογραφίας: [κανόνες ροής αλληλογραφίας (κανόνες μεταφοράς) στο Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)

- Κανόνες ροής αλληλογραφίας εγκατάστασης: [διαδικασίες κανόνα ροής αλληλογραφίας στο Exchange Online](https://technet.microsoft.com/library/dn600436.aspx)

- Δημιουργία, τροποποίηση και διαγραφή κανόνων ροής αλληλογραφίας: [Διαχείριση κανόνων ροής αλληλογραφίας](https://technet.microsoft.com/library/jj657505.aspx)

Μπορείτε επίσης να διαχειριστείτε κανόνες ροής αλληλογραφίας στο Exchange Online PowerShell. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Get-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (View), [New-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (Create), [Remove-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (Delete), [TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (Modify υπάρχοντα), [disable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (απενεργοποίηση υπάρχουσας) και [Enable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (Ενεργοποίηση υπάρχοντος).

Πρόσθετα cmdlet κανόνα ροής αλληλογραφίας: [Get-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (λίστα διαθέσιμες ενέργειες), [Get-TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (λίστα διαθέσιμων συνθηκών και εξαιρέσεων), [εξαγωγή-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (κανόνες εξαγωγής) και [Import-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (κανόνες εισαγωγής).
