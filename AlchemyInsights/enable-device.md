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
ms.openlocfilehash: 4722ccf6847fc6c02616dbc62d59a2a87c089f77ae79c0a916211af6c5f2a6d0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54003484"
---
# <a name="enable-device"></a>Ενεργοποίηση συσκευής

**Για να ενεργοποιήσετε τη συσκευή χρησιμοποιώντας την εντολή Powershell**

Εκτελέστε τις παρακάτω εντολές:

- Για να λάβετε ένα αντικείμενο συσκευής: `Get-MsolDevice -Name <Name>`
- Για να ενεργοποιήσετε τη συσκευή: `Enable-MsolDevice -DeviceId <DeviceId>`

Για περισσότερες πληροφορίες σχετικά με τη ρύθμιση παραμέτρων υβριδικής συμμετοχής σε διαχειριζόμενους τομείς, ανατρέξτε στο θέμα [Ρύθμιση παραμέτρων υβριδικής συμμετοχής.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains)
