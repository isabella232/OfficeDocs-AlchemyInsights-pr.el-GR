---
title: Θύρα Google Chrome Extensions στο Microsoft Edge (χρώμιο)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004032"
- "7102"
ms.openlocfilehash: 2a20f258cbcbca7c8db4e38c52464fefb1b6f39d
ms.sourcegitcommit: 38c87ed786dda7181562492d5d2e7ef0e18e0cab
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677882"
---
# <a name="port-google-chrome-extensions-to-microsoft-edge-chromium"></a><span data-ttu-id="e67b8-102">Θύρα Google Chrome Extensions στο Microsoft Edge (χρώμιο)</span><span class="sxs-lookup"><span data-stu-id="e67b8-102">Port Google Chrome extensions to Microsoft Edge (Chromium)</span></span>

<span data-ttu-id="e67b8-103">Είναι εύκολο να [μεταφέρετε επεκτάσεις του Google Chrome στο Microsoft Edge (χρώμιο)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension).</span><span class="sxs-lookup"><span data-stu-id="e67b8-103">It's easy to [port Google Chrome extensions to Microsoft Edge (Chromium)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension).</span></span> <span data-ttu-id="e67b8-104">Στις περισσότερες περιπτώσεις, απαιτούνται μόνο ελάχιστες αλλαγές για την εκτέλεση αυτών των επεκτάσεων στο Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="e67b8-104">In most cases, only minimal changes are needed to run these extensions on Microsoft Edge.</span></span>

<span data-ttu-id="e67b8-105">Τα API επεκτάσεων και τα κλειδιά διακηρύξεων που υποστηρίζονται από το Google Chrome είναι συμβατά με τον κώδικα με το Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="e67b8-105">The extension APIs and manifest keys supported by Google Chrome are code-compatible with Microsoft Edge.</span></span> <span data-ttu-id="e67b8-106">Ωστόσο, το Microsoft Edge δεν υποστηρίζει τα API επεκτάσεων Chrome. GCM, Chrome. Identity. getAccounts, Chrome. Identity. getAuthToken και Chrome. εμφάνισης.</span><span class="sxs-lookup"><span data-stu-id="e67b8-106">However, Microsoft Edge does not support the extension APIs chrome.gcm, chrome.identity.getAccounts, chrome.identity.getAuthToken, and chrome.instanceID.</span></span>