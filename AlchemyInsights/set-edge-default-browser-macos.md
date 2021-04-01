---
title: Ορισμός του Microsoft Edge ως προεπιλεγμένου προγράμματος περιήγησης σε συσκευή macOS
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: 5318c7d20ee7091e162e566cd2b4ebf5d255915b
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/30/2021
ms.locfileid: "51491553"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-macos-device"></a>Ορισμός του Microsoft Edge ως προεπιλεγμένου προγράμματος περιήγησης σε συσκευή macOS

Χρησιμοποιήστε μία από αυτές τις δύο μεθόδους για να ορίσετε τον Microsoft Edge ως το προεπιλεγμένο πρόγραμμα περιήγησης:

Μέθοδος 1: Αναβοσβήνουν τη συσκευή με μια εικόνα του macOS όπου ο Microsoft Edge έχει ήδη οριστεί ως το προεπιλεγμένο πρόγραμμα περιήγησης.

Μέθοδος 2: Ορίστε την πολιτική DefaultBrowserSettingEnabled ώστε να ζητά από το χρήστη να ορίσει τον Microsoft Edge ως το προεπιλεγμένο πρόγραμμα περιήγησης.

Οποιαδήποτε από τις δύο μεθόδους επιτρέπει σε ένα χρήστη να αλλάξει το προεπιλεγμένο πρόγραμμα περιήγησης. Για το λόγο αυτό, συνιστάται να αναπτύξετε την πολιτική DefaultBrowserSettingEnabled ακόμα και αν χρησιμοποιήσατε τη μέθοδο 1. Εάν ένας χρήστης αλλάξει το προεπιλεγμένο πρόγραμμα περιήγησης μετά την ανάπτυξη της πολιτικής, η πολιτική ζητά από το χρήστη να ορίσει ξανά το προεπιλεγμένο πρόγραμμα περιήγησης στον Microsoft Edge.
