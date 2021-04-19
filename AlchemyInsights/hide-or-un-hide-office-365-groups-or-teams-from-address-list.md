---
title: Απόκρυψη ή κατάργηση απόκρυψης ομάδων ή ομάδων του Office 365 από τη λίστα διευθύνσεων
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
- "9002947"
- "5642"
ms.openlocfilehash: 12e221c69775f3dfeed1781b70d3061e1ca0ac3b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51811456"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a>Απόκρυψη ή κατάργηση απόκρυψης ομάδων ή ομάδων του Office 365 από τη λίστα διευθύνσεων

Χρησιμοποιήστε την ακόλουθη εντολή EXO PowerShell για να αποκρύψετε ή να αποκρύψετε την ομάδα/ομάδες του Office 365 από λίστες διευθύνσεων (GAL) των πελατών του Exchange (Outlook, OWA):

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

Χρησιμοποιήστε την ακόλουθη εντολή EXO PowerShell για να αποκρύψετε ή να αποκρύψετε την ομάδα/ομάδες του Office365 από προγράμματα-πελάτες του Exchange (Outlook, OWA):

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- Για λεπτομερείς οδηγίες, ανατρέξτε [στο θέμα Απόκρυψη ομάδων του Office 365 από τα προγράμματα-πελάτες GAL και Exchange.](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal)
