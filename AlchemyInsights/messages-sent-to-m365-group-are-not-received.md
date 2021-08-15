---
title: Τα μηνύματα που αποστέλλονται στην ομάδα Microsoft 365 δεν λαμβάνονται από όλα τα μέλη
ms.author: pebaum
author: pebaum
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: 73c0fd3eb2f022b1c5917849bae676b748025fb69a3a15ba1389b42a6854db9c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53976505"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a>Τα μηνύματα που αποστέλλονται σε μια ομάδα του Microsoft 365 δεν λαμβάνονται από όλα τα μέλη

Βεβαιωθείτε ότι όλα τα μέλη της ομάδας έχουν εγγραφεί για να λαμβάνουν τα μηνύματα ηλεκτρονικού ταχυδρομείου. Ανατρέξτε στο θέμα [Παρακολούθηση ομάδας στο Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).  

Για να ελέγξετε την κατάσταση μηνυμάτων των μελών που έχουν εγγραφεί στα μηνύματα ηλεκτρονικού ταχυδρομείου ομάδας, εκτελέστε την ακόλουθη εντολή [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true):

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`

Χρησιμοποιήστε την παρακάτω εντολή EXO PowerShell για να ρυθμίσετε τις παραμέτρους όλων των μελών της ομάδας, ώστε να λαμβάνουν μηνύματα ηλεκτρονικού ταχυδρομείου που αποστέλλονται στην ομάδα Microsoft 365 στα εισερχόμενά τους:

`$Group = "Address of [Microsoft 365 Groups]"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`

Για παράδειγμα:

`$Group = "testg@contoso.onmicrosoft.com"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`