---
title: Ενεργοποίηση τεχνολογίας NDI
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
- "9004403"
- "7947"
ms.openlocfilehash: ea694898baffa50fca71957175eba3664dece44e
ms.sourcegitcommit: 112f18dce8257b98fab32d44910ee879efb44cb8
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935101"
---
# <a name="turn-on-ndi-technology"></a>Ενεργοποίηση τεχνολογίας NDI

Η τεχνολογία NDI απαιτεί δύο βήματα για να ενεργοποιηθεί για ένα χρήστη:

1. Ο διαχειριστής μισθωτή πρέπει να ενεργοποιήσει την ιδιότητα "AllowNDIStreaming" στο CsTeamsMeetingPolicy.

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. Αφού συμπληρωθεί αυτή η αλλαγή, ο τελικός χρήστης πρέπει να ® NDI για το συγκεκριμένο πρόγραμμα-πελάτη από τις **Ρυθμίσεις > δικαιώματα.**

Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα "Χρήση της τεχνολογίας NDI στο Microsoft Teams".](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings)
