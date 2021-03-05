---
title: Απενεργοποίηση σάρωσης δικτύου
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001464"
- "3492"
ms.openlocfilehash: 7b0f5c21a7e6afda0ee3000e75ee725cbadcedb7
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481399"
---
# <a name="disable-network-scan"></a><span data-ttu-id="a6ccb-102">Απενεργοποίηση σάρωσης δικτύου</span><span class="sxs-lookup"><span data-stu-id="a6ccb-102">Disable network scan</span></span>

<span data-ttu-id="a6ccb-103">Οι σαρώσεις κοινής χρήσης δικτύου ενδέχεται να επηρεάσουν τις επιδόσεις.</span><span class="sxs-lookup"><span data-stu-id="a6ccb-103">Network share scans may impact performance.</span></span>  <span data-ttu-id="a6ccb-104">Για να εξασφαλίσετε ότι το πρόγραμμα-πελάτης δεν σαρώνει κοινόχρηστα στοιχεία δικτύου/αρχεία από προεπιλογή, ρυθμίστε τις παραμέτρους των ακόλουθων ρυθμίσεων στην εφαρμογή Windows Defender στην **τιμή True:**</span><span class="sxs-lookup"><span data-stu-id="a6ccb-104">To ensure the client does not scan network shares/files by default, configure the following settings in the Windows Defender application to **True**:</span></span>

- <span data-ttu-id="a6ccb-105">DisableScanningMappedNetworkDrivesForFullScan</span><span class="sxs-lookup"><span data-stu-id="a6ccb-105">DisableScanningMappedNetworkDrivesForFullScan</span></span>
- <span data-ttu-id="a6ccb-106">DisableScanningNetworkFiles</span><span class="sxs-lookup"><span data-stu-id="a6ccb-106">DisableScanningNetworkFiles</span></span>