---
title: Τα επίπεδα δικαιωμάτων του SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 356fef8e02f2c1fd9d209c68194685bb0acaa367
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760693"
---
# <a name="sharepoint-designer-connection-issues"></a>Προβλήματα σύνδεσης του SharePoint Designer 

Εάν το SharePoint Designer αντιμετωπίζει ζητήματα σύνδεσης σε τοποθεσίες του SharePoint, προσπαθήστε τις ακόλουθες κοινές λύσεις.

Βήμα 1: Βεβαιωθείτε ενημερώνεται το SharePoint Designer.

- [Του SharePoint Designer 2013](https://www.microsoft.com/download/details.aspx?id=35491)

- [Το SharePoint Designer Service Pack 1 (SP1)](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)

- [Ενημερωμένη έκδοση για το SharePoint Designer 2013 (KB3114721)](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)

Βήμα 2: Καταργήστε το τοπικό χώρο προσωρινής αποθήκευσης αρχείων

- Κλείσιμο του SharePoint Designer 2013.

- Στον τοπικό υπολογιστή, μεταβείτε στους ακόλουθους φακέλους για να καταργήσετε προσωρινά αποθηκευμένα αρχεία.

- Κάντε κλικ στο κουμπί Έναρξη, εκτέλεση "και" Διαγραφή όλων των αρχείων που βρέθηκαν σε κάθε μία από τις παρακάτω θέσεις.

Διακομιστής %APPDATA%\Microsoft\Web Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

Άνοιγμα του SharePoint Designer 2013 και εισαγάγετε το λογαριασμό ξανά, για να δείτε αν λειτουργεί.

Βήμα 3: [Ενεργοποίηση σύγχρονη ελέγχου ταυτότητας για το Office 2013 σε συσκευές των Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)

Βήμα 4: Οι διαχειριστές θα πρέπει να επιτρέψει προσαρμοσμένης δέσμης ενεργειών επιτρέπουν τη σύνδεση του SharePoint Designer.

Για λεπτομερή βήματα, παραδείγματα και ζητήματα, δείτε [επιτρέπεται ή να απαγορεύεται η προσαρμοσμένη δέσμη ενεργειών](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


