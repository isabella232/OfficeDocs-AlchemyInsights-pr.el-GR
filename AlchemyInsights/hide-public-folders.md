---
title: Απόκρυψη δημόσιων φακέλων
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "8417"
ms.openlocfilehash: 70179296e9c1bb7391535f55796bc5af80b825f8
ms.sourcegitcommit: a019bd8b0244914edb59e124bc6538cdc5c158f9
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 02/18/2021
ms.locfileid: "50315370"
---
# <a name="hide-public-folders"></a><span data-ttu-id="c4d6c-102">Απόκρυψη δημόσιων φακέλων</span><span class="sxs-lookup"><span data-stu-id="c4d6c-102">Hide public folders</span></span>

<span data-ttu-id="c4d6c-103">**Για να αποκρύψετε ολόκληρο το δέντρο δημόσιων φακέλων:**</span><span class="sxs-lookup"><span data-stu-id="c4d6c-103">**To hide entire public folder tree**:</span></span>

<span data-ttu-id="c4d6c-104">Χρησιμοποιήστε τα βήματα σε αυτό [το άρθρο για](https://aka.ms/ControlPF) να αποκρύψετε ολόκληρο το δέντρο δημόσιων φακέλων από επιλεκτικούς ή όλους τους χρήστες.</span><span class="sxs-lookup"><span data-stu-id="c4d6c-104">Use the steps in [this](https://aka.ms/ControlPF) article to hide entire public folder tree from selective or all users.</span></span>

<span data-ttu-id="c4d6c-105">**Για να αποκρύψετε έναν συγκεκριμένο δημόσιο φάκελο:**</span><span class="sxs-lookup"><span data-stu-id="c4d6c-105">**To hide a specific public folder**:</span></span>

1. <span data-ttu-id="c4d6c-106">Προσθήκη δικαιωμάτων για χρήστες που πρέπει να έχουν πρόσβαση στον δημόσιο φάκελο</span><span class="sxs-lookup"><span data-stu-id="c4d6c-106">Add permissions for users who need to access the public folder</span></span>

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. <span data-ttu-id="c4d6c-107">Κατάργηση της προεπιλογής **χρήστη** από τη **λίστα δικαιωμάτων:**</span><span class="sxs-lookup"><span data-stu-id="c4d6c-107">Remove the user **Default** from the **permission** list:</span></span>

    `Remove-PublicFolderClientPermission \test1 -User Default`
