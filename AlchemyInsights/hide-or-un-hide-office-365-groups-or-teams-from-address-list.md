---
title: Απόκρυψη ή κατάργηση απόκρυψης Office 365 ομάδων ή ομάδων από τη λίστα διευθύνσεων
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
ms.openlocfilehash: 7e667e22cd81f38a1a2c1385bf42e5227cb641480f4b505110ee7349a13f13a1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088396"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a>Απόκρυψη ή κατάργηση απόκρυψης Office 365 ομάδων ή ομάδων από τη λίστα διευθύνσεων

Χρησιμοποιήστε την ακόλουθη εντολή EXO PowerShell για να αποκρύψετε ή να αποκρύψετε την ομάδα/ομάδες Office 365 από λίστες διευθύνσεων (GAL) Exchange πελατών (Outlook, OWA):

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

Χρησιμοποιήστε την ακόλουθη εντολή EXO PowerShell για να αποκρύψετε ή να αποκρύψετε την ομάδα/ομάδες του Office365 από προγράμματα-πελάτες Exchange (Outlook, OWA):

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- Για λεπτομερείς οδηγίες, [ανατρέξτε στο θέμα Απόκρυψη Office 365 ομάδων από το GAL και Exchange πελάτες.](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal)
