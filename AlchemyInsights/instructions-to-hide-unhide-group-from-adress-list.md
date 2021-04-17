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
ms.openlocfilehash: 4d55866700b9b8494f1f692cd3b865116b96a1bc
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831878"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Απόκρυψη της ομάδας Microsoft 365 από τη λίστα διευθύνσεων (GAL)

Για να αποκρύψετε μια ομάδα Microsoft 365 από λίστες διευθύνσεων (GAL) των πελατών του Exchange (όπως το Outlook ή το OWA), χρησιμοποιήστε την ακόλουθη εντολή στο κέλυφος EXO:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Για να αποκρύψετε την ομάδα Microsoft 365 από το να είναι ορατή στα προγράμματα-πελάτες του Exchange, χρησιμοποιήστε την ακόλουθη εντολή στο κέλυφος EXO:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

