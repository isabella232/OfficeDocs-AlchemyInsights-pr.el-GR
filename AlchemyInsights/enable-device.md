---
title: Ενεργοποίηση συσκευής
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "8278"
ms.openlocfilehash: 9e4b03dcba7a2c98a5d63213ee49f9ba8f91d670
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256761"
---
# <a name="enable-device"></a>Ενεργοποίηση συσκευής

**Για να ενεργοποιήσετε τη συσκευή χρησιμοποιώντας την εντολή Powershell**

Εκτελέστε τις παρακάτω εντολές:

- Για να λάβετε ένα αντικείμενο συσκευής: `Get-MsolDevice -Name <Name>`
- Για να ενεργοποιήσετε τη συσκευή: `Enable-MsolDevice -DeviceId <DeviceId>`

Για περισσότερες πληροφορίες σχετικά με τη ρύθμιση παραμέτρων υβριδικού συνδέσμου σε διαχειριζόμενους τομείς, ανατρέξτε στο θέμα "Ρύθμιση [παραμέτρων υβριδικού συνδέσμου".](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains)
