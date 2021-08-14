---
title: SharePoint Προβλήματα σύνδεσης με το πρόγραμμα σχεδίασης
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
ms.openlocfilehash: d55f7c1902bb623900fa74bdae70695b6e04ad84ce7b6ea314db614283ec436d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53942025"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Προβλήματα σύνδεσης με το πρόγραμμα σχεδίασης 

Εάν SharePoint Designer αντιμετωπίζει προβλήματα σύνδεσης με SharePoint τοποθεσίες, δοκιμάστε τις παρακάτω κοινές λύσεις.

Βήμα 1: Βεβαιωθείτε ότι το SharePoint Designer 2013 έχει ενημερωθεί με [το SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) και την Ενημέρωση [2 Αυγούστου 2016 για το SharePoint Designer 2013.](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)



Βήμα 2: Απαλοιφή των τοπικών αρχείων cache:

1. Κλείστε SharePoint Designer 2013.

2. Στον τοπικό υπολογιστή, καταργήστε όλα τα αρχεία που βρίσκονται σε κάθε έναν από τους ακόλουθους φακέλους.

    - %APPDATA%\Microsoft\Web Server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Ανοίξτε SharePoint Designer 2013 και πληκτρολογήστε ξανά το λογαριασμό για να δείτε εάν λειτουργεί.

Βήμα 3: [Ενεργοποίηση σύγχρονου ελέγχου ταυτότητας για Office 2013 σε Windows συσκευές.](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)

Βήμα 4: Οι διαχειριστές  θα πρέπει να επιτρέψουν την προσαρμοσμένη δέσμη ενεργειών στις SharePoint του Κέντρου διαχείρισης για να επιτρέψουν τη σύνδεση SharePoint Σχεδίασης. Ανατρέξτε [στο θέμα Αποδοχή ή αποτροπή προσαρμοσμένης δέσμης](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) ενεργειών για περισσότερες πληροφορίες.


