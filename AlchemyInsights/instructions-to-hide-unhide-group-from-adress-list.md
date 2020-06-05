---
title: Οδηγίες απόκρυψης/επανεμφάνισης ομάδας από τη λίστα διευθύνσεων
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 02368d6a06df90d76ee1bd5448819e7ffe12c18c
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580009"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Απόκρυψη ομάδας microsoft 365 από τη λίστα διευθύνσεων (GAL)

Για να αποκρύψετε μια ομάδα Microsoft 365 από λίστες διευθύνσεων (GAL) υπολογιστών-πελατών του Exchange (όπως το Outlook ή το OWA), χρησιμοποιήστε την ακόλουθη εντολή στο κέλυφος EXO:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Για να αποκρύψετε την ορατή ομάδα Microsoft 365 σε υπολογιστές-πελάτες του Exchange, χρησιμοποιήστε την ακόλουθη εντολή στο κέλυφος EXO:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

