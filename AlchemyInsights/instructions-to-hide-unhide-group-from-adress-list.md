---
title: Οδηγίες απόκρυψης/εμφάνισης ομάδας από τη λίστα διευθύνσεων
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: af7085890d295cf0c41e11aaf18e404313413100cb8a1134bfac051d5fa26996
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53926245"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Απόκρυψη Microsoft 365 ομάδας από τη λίστα διευθύνσεων (GAL)

Για να αποκρύψετε μια Microsoft 365 από λίστες διευθύνσεων (GAL) των πελατών Exchange (όπως το Outlook ή το OWA), χρησιμοποιήστε την ακόλουθη εντολή στο κέλυφος EXO:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Για να αποκρύψετε Microsoft 365 ομάδας από το να είναι ορατή Exchange προγράμματα-πελάτες, χρησιμοποιήστε την ακόλουθη εντολή στο κέλυφος EXO:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

