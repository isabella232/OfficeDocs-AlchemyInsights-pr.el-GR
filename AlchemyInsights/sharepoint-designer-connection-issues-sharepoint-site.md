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
ms.openlocfilehash: 7451cfe957545537298f57feb5b47bd6d43cddbf
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/04/2019
ms.locfileid: "34716892"
---
# <a name="sharepoint-designer-connection-issues"></a>Προβλήματα σύνδεσης του SharePoint Designer 

<p>Εάν το SharePoint Designer αντιμετωπίζει ζητήματα σύνδεσης σε τοποθεσίες του SharePoint, προσπαθήστε τις ακόλουθες κοινές λύσεις.</p> <p><strong>Βήμα 1:</strong> <strong>Ενημερώνεται η επαλήθευση του SharePoint Designer&nbsp; </strong></p> <ul> <li><a href="https://www.microsoft.com/en-us/download/details.aspx?id=35491">Του SharePoint Designer 2013</a></li> <li><a href="https://support.microsoft.com/en-us/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1">Το SharePoint Designer Service Pack 1 (SP1)</a></li> <li><a href="https://support.microsoft.com/en-us/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721">Ενημερωμένη έκδοση για το SharePoint Designer 2013 (KB3114721)</a></li> </ul> <p><strong>Βήμα 2:</strong> <strong>Καταργήστε το τοπικό χώρο προσωρινής αποθήκευσης αρχείων</strong>&nbsp;</p> <ol> <li style="font-weight: 400;">Κλείσιμο του SharePoint Designer 2013.&nbsp;</li> <li style="font-weight: 400;">Στον τοπικό υπολογιστή, μεταβείτε στους ακόλουθους φακέλους για να καταργήσετε προσωρινά αποθηκευμένα αρχεία.&nbsp;</li> <li style="font-weight: 400;">Κάντε κλικ στο κουμπί <strong>εκκίνηση -&gt; εκτέλεση</strong> και διαγράψτε όλα τα αρχεία που βρέθηκαν σε κάθε μία από τις παρακάτω θέσεις.&nbsp;<br /><br />Extensions\Cache διακομιστής %APPDATA%\Microsoft\Web<br />%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache<br />%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</li> <li style="font-weight: 400;">Άνοιγμα του SharePoint Designer 2013 και εισαγάγετε το λογαριασμό ξανά, για να δείτε αν λειτουργεί.</li> </ol> <p><strong>Βήμα 3:</strong> <a href="https://docs.microsoft.com/en-us/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=%252fen-us%252farticle%252fEnable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&amp;view=o365-worldwide"> <strong>Ενεργοποίηση σύγχρονη ελέγχου ταυτότητας για το Office 2013 σε συσκευές των Windows</strong></a>&nbsp;</p> <p><strong>Βήμα 4:</strong> <strong>Οι διαχειριστές θα πρέπει να επιτρέψει προσαρμοσμένης δέσμης ενεργειών για να επιτρέπεται η σύνδεση του SharePoint Designer</strong>.</p> <p>Για λεπτομερή βήματα, παραδείγματα και ζητήματα, δείτε <a href="https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script">επιτρέπεται ή να απαγορεύεται η προσαρμοσμένη δέσμη ενεργειών</a>.&nbsp;</p>


