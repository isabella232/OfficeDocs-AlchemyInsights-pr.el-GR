---
title: Οδηγίες για απόκρυψη/επανεμφάνιση ομάδας από τη λίστα διευθύνσεων
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 1ad9ab294d46ca0fc88a454e3503ddcf80398896
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663009"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a><span data-ttu-id="f2298-102">Απόκρυψη της ομάδας Microsoft 365 από τη λίστα διευθύνσεων (GAL)</span><span class="sxs-lookup"><span data-stu-id="f2298-102">Hide Microsoft 365 group from address list (GAL)</span></span>

<span data-ttu-id="f2298-103">Για να αποκρύψετε μια ομάδα του Microsoft 365 από λίστες διευθύνσεων (GAL) των προγραμμάτων-πελατών του Exchange (όπως το Outlook ή το OWA), χρησιμοποιήστε την ακόλουθη εντολή στο έξω κέλυφος:</span><span class="sxs-lookup"><span data-stu-id="f2298-103">To hide a Microsoft 365 group from address lists (GAL) of Exchange clients (such as Outlook or OWA), use the following command in EXO shell:</span></span>

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

<span data-ttu-id="f2298-104">Για να αποκρύψετε την ομάδα του Microsoft 365 από το να είναι ορατή σε προγράμματα-πελάτες του Exchange, χρησιμοποιήστε την ακόλουθη εντολή στο έξω κέλυφος:</span><span class="sxs-lookup"><span data-stu-id="f2298-104">To hide the Microsoft 365 group from being visible to Exchange clients, use the following command in EXO shell:</span></span>

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

