---
title: Ζητήματα σύνδεσης σχεδίασης του SharePoint
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
ms.openlocfilehash: 01ccc6bc28148f397fb6cd2b7a0eaaeb5b51973f
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511544"
---
# <a name="sharepoint-designer-connection-issues"></a>Ζητήματα σύνδεσης σχεδίασης του SharePoint 

Εάν το SharePoint Designer αντιμετωπίζει προβλήματα σύνδεσης σε τοποθεσίες του SharePoint, δοκιμάστε τις ακόλουθες κοινές λύσεις.

Βήμα 1: Βεβαιωθείτε ότι το SharePoint Designer 2013 ενημερώνεται με το [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) και την ενημερωμένη έκδοση 2 [Αυγούστου 2016 για το SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Βήμα 2: Απαλοιφή των τοπικών αρχείων προσωρινής αποθήκευσης:

1. Κλείστε το SharePoint Designer 2013.

2. Στον τοπικό υπολογιστή, καταργήστε όλα τα αρχεία που βρίσκονται σε κάθε έναν από τους ακόλουθους φακέλους.

    - %APPDATA%\Επεκτάσεις διακομιστή Web\Cache
    - %APPDATA%\Microsoft\Σχεδιαστής του SharePoint\Cache συγκρότησης διακομιστή μεσολάβησης
    - %ΠΡΟΦΊΛ ΧΡΗΣΤΗΣ%\Δεδομένα εφαρμογών\Τοπικές\Microsoft\Cache τοποθεσιών Web

3. Ανοίξτε το SharePoint Designer 2013 και πληκτρολογήστε ξανά το λογαριασμό για να δείτε αν λειτουργεί.

Βήμα 3: [Ενεργοποίηση σύγχρονου ελέγχου ταυτότητας για το Office 2013 σε συσκευές των Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).

Βήμα 4: Οι διαχειριστές θα πρέπει να **επιτρέψουν την προσαρμοσμένη δέσμη ενεργειών** στις ρυθμίσεις του Κέντρου διαχείρισης του SharePoint για να επιτρέψουν τη σύνδεση του SharePoint Designer. Ανατρέξτε [στο θέμα Να επιτρέπεται ή να αποτρέπεται η προσαρμοσμένη δέσμη ενεργειών](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) για περισσότερες πληροφορίες.


