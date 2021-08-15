---
title: Ενεργοποίηση της τεχνολογίας NDI
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
ms.openlocfilehash: ed932592aae1158bc0c0da4817467b69d20208533bc080cb0e424f552af8601a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54023522"
---
# <a name="turn-on-ndi-technology"></a>Ενεργοποίηση της τεχνολογίας NDI

Η τεχνολογία NDI απαιτεί να είναι ενεργοποιημένα δύο βήματα για ένα χρήστη:

1. Ο διαχειριστής μισθωτή πρέπει να ενεργοποιήσει την ιδιότητα "AllowNDIStreaming" στο CsTeamsMeetingPolicy.

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. Μετά τη συμπλήρωση αυτής της αλλαγής, ο τελικός χρήστης πρέπει να ενεργοποιήσετε την τεχνολογία NDI® για το συγκεκριμένο **πρόγραμμα-πελάτη από Ρυθμίσεις > δικαιώματα.**

Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα Χρήση της τεχνολογίας NDI Microsoft Teams.](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings)
