---
title: Προβλήματα σύνδεσης του SharePoint Designer
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 997ba3de58485d4fe6d24b926c33348378af8cd3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727171"
---
# <a name="sharepoint-designer-connection-issues"></a>Προβλήματα σύνδεσης του SharePoint Designer 

Εάν το SharePoint Designer αντιμετωπίζει προβλήματα σύνδεσης σε τοποθεσίες του SharePoint, δοκιμάστε τις παρακάτω συνηθισμένες λύσεις.

Βήμα 1: Επαληθεύστε ότι το SharePoint Designer 2013 ενημερώνεται με το [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) και την [ενημέρωση 2 Αυγούστου 2016 για το sharepoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Βήμα 2: Καταργήστε την εκκαθάριση των αρχείων της τοπικής μνήμης cache:

1. Κλείστε το SharePoint Designer 2013.

2. Στον τοπικό υπολογιστή, καταργήστε όλα τα αρχεία που βρίσκονται σε κάθε έναν από τους παρακάτω φακέλους.

    - %APPDATA%\Microsoft\Web Server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Ανοίξτε το SharePoint Designer 2013 και εισαγάγετε ξανά τον λογαριασμό για να δείτε εάν λειτουργεί.

Βήμα 3: [Ενεργοποίηση του σύγχρονου ελέγχου ταυτότητας για το Office 2013 σε συσκευές Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).

Βήμα 4: οι διαχειριστές θα πρέπει να **επιτρέψουν την προσαρμοσμένη δέσμη ενεργειών** στις ρυθμίσεις του κέντρου διαχείρισης του SharePoint, ώστε να επιτρέπεται η σύνδεση του SharePoint Designer. Ανατρέξτε στο θέμα να [επιτρέπεται ή να εμποδίζεται η προσαρμοσμένη δέσμη ενεργειών](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) για περισσότερες πληροφορίες.


