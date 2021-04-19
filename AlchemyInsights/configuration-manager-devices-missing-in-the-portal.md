---
title: Συσκευές Configuration Manager που λείπουν από την πύλη
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
- "9001495"
- "4384"
ms.openlocfilehash: d57659eb928dd8c4653499e65b6e6cd2f021f521
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817244"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a><span data-ttu-id="6cb0a-102">Συσκευές Configuration Manager που λείπουν από την πύλη</span><span class="sxs-lookup"><span data-stu-id="6cb0a-102">Configuration Manager devices missing in the portal</span></span>

<span data-ttu-id="6cb0a-103">Για να λειτουργήσει ο συγχρονισμός συσκευής, τα [απαιτούμενα τελικά σημεία Internet](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) πρέπει να είναι προσβάσιμα από τον διακομιστή εσωτερικής εγκατάστασης που φιλοξενεί τον ρόλο Σημείο σύνδεσης υπηρεσίας.</span><span class="sxs-lookup"><span data-stu-id="6cb0a-103">For device sync to work, [required internet endpoints](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) must be reachable from the on-premise server hosting the Service Connection Point role.</span></span> <span data-ttu-id="6cb0a-104">Για την αντιμετώπιση προβλημάτων με τον συγχρονισμό συσκευών, ελέγξτε το **CMGatewaySyncUploadWorker.log** που βρίσκεται στο σημείο σύνδεσης της υπηρεσίας.</span><span class="sxs-lookup"><span data-stu-id="6cb0a-104">To troubleshoot device sync, please review the **CMGatewaySyncUploadWorker.log** located on the service connection point.</span></span>

<span data-ttu-id="6cb0a-105">Μάθετε περισσότερα σχετικά με την [Επισύναψη μισθωτή στο Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).</span><span class="sxs-lookup"><span data-stu-id="6cb0a-105">Learn more about [Tenant attach in Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).</span></span>
