---
title: Αποκλεισμός λήψης σε συνδέσεις κοινής χρήσης
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000213"
- "5715"
ms.openlocfilehash: 8cb53754125cedf4a3d0426d6c3bf70297eb3d74
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 05/23/2020
ms.locfileid: "44357627"
---
# <a name="block-download-on-sharing-links"></a>Αποκλεισμός λήψης σε συνδέσεις κοινής χρήσης

**Η λήψη αποκλεισμού** είναι διαθέσιμη για **συνδέσεις μόνο για προβολή σε** έγγραφα του Office. Όταν κάνετε αυτήν την επιλογή, τα άτομα που αποκτούν πρόσβαση στο αρχείο μέσω της σύνδεσης που δημιουργήσατε δεν θα βλέπουν επιλογές λήψης, εκτύπωσης ή αντιγραφής του αρχείου.

Οι διαχειριστές μπορούν να ελέγξουν εάν η ρύθμιση "αποκλεισμός λήψης" θα εμφανίζεται μόνο για αρχεία του Office ή όχι, αλλάζοντας `BlockDownloadLinksFileType` τη ρύθμιση στα cmdlets [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps) ή [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) PowerShell.
