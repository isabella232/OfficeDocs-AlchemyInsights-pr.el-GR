---
title: Οδηγίες για την απόκρυψη/επανεμφάνιση ομάδας από τη λίστα διευθύνσεων
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
ms.openlocfilehash: d0e0285701f1a5f308bdc682abaddf5cc2d34120
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768922"
---
# <a name="hide-office-365-group-from-address-list-gal"></a>Απόκρυψη ομάδας Office 365 από τη λίστα διευθύνσεων (GAL)

Για να αποκρύψετε μια ομάδα Office 365 από λίστες διευθύνσεων (GAL) των προγραμμάτων-πελατών του Exchange (όπως το Outlook ή το OWA), χρησιμοποιήστε την ακόλουθη εντολή στο κέλυφος εξω:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Για να αποκρύψετε την ομάδα Office 365 από το να είναι ορατή σε προγράμματα-πελάτες του Exchange, χρησιμοποιήστε την ακόλουθη εντολή στο κέλυφος εξω:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

