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
# <a name="hide-public-folders"></a>Απόκρυψη δημόσιων φακέλων

**Για να αποκρύψετε ολόκληρο το δέντρο δημόσιων φακέλων:**

Χρησιμοποιήστε τα βήματα σε αυτό [το άρθρο για](https://aka.ms/ControlPF) να αποκρύψετε ολόκληρο το δέντρο δημόσιων φακέλων από επιλεκτικούς ή όλους τους χρήστες.

**Για να αποκρύψετε έναν συγκεκριμένο δημόσιο φάκελο:**

1. Προσθήκη δικαιωμάτων για χρήστες που πρέπει να έχουν πρόσβαση στον δημόσιο φάκελο

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. Κατάργηση της προεπιλογής **χρήστη** από τη **λίστα δικαιωμάτων:**

    `Remove-PublicFolderClientPermission \test1 -User Default`
