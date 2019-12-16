---
title: Ζητήματα σύνδεσης του SharePoint Designer
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 9730bd66afd494385db3de605f5fe68d0f274ed3
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051713"
---
# <a name="sharepoint-designer-connection-issues"></a>Ζητήματα σύνδεσης του SharePoint Designer 

Εάν το SharePoint Designer αντιμετωπίζει ζητήματα σύνδεσης σε τοποθεσίες του SharePoint, δοκιμάστε τις ακόλουθες κοινές λύσεις.

Βήμα 1: Επαληθεύστε ότι το SharePoint Designer 2013 ενημερώνεται με το [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) και το [2 Αυγούστου, 2016 ενημερωμένη έκδοση για το SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Βήμα 2: απαλοιφή των αρχείων τοπικής μνήμης cache:

1. Κλείστε το SharePoint Designer 2013.

2. Στον τοπικό υπολογιστή, καταργήστε όλα τα αρχεία που βρίσκονται σε καθέναν από τους ακόλουθους φακέλους.

    - %AppData%\micssoft\ ρυθμίσεις διακομιστή Web \ cache
    - %Appdats\micsss\ σχεδίαση
    - %Profile\applods\sooms\ μικρολογισμικός

3. Ανοίξτε το SharePoint Designer 2013 και εισαγάγετε ξανά το λογαριασμό για να δείτε αν λειτουργεί.

Βήμα 3: [Ενεργοποίηση σύγχρονου ελέγχου ταυτότητας για το Office 2013 σε συσκευές Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).

Βήμα 4: οι διαχειριστές θα πρέπει να **επιτρέψετε προσαρμοσμένη δέσμη ενεργειών** στις ρυθμίσεις του κέντρου διαχείρισης του SharePoint για να επιτρέψετε τη σύνδεση του SharePoint Designer. Δείτε να [επιτρέπεται ή να αποτρέπεται η προσαρμοσμένη δέσμη ενεργειών](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) για περισσότερες πληροφορίες.


