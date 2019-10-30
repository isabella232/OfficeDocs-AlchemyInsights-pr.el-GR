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
# <a name="hide-office-365-group-from-address-list-gal"></a><span data-ttu-id="244e1-102">Απόκρυψη ομάδας Office 365 από τη λίστα διευθύνσεων (GAL)</span><span class="sxs-lookup"><span data-stu-id="244e1-102">Hide Office 365 group from address list (GAL)</span></span>

<span data-ttu-id="244e1-103">Για να αποκρύψετε μια ομάδα Office 365 από λίστες διευθύνσεων (GAL) των προγραμμάτων-πελατών του Exchange (όπως το Outlook ή το OWA), χρησιμοποιήστε την ακόλουθη εντολή στο κέλυφος εξω:</span><span class="sxs-lookup"><span data-stu-id="244e1-103">To hide an Office 365 group from address lists (GAL) of Exchange clients (such as Outlook or OWA), use the following command in EXO shell:</span></span>

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

<span data-ttu-id="244e1-104">Για να αποκρύψετε την ομάδα Office 365 από το να είναι ορατή σε προγράμματα-πελάτες του Exchange, χρησιμοποιήστε την ακόλουθη εντολή στο κέλυφος εξω:</span><span class="sxs-lookup"><span data-stu-id="244e1-104">To hide the Office 365 group from being visible to Exchange clients, use the following command in EXO shell:</span></span>

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

