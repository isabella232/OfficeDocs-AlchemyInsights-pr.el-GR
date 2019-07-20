---
title: Δεν υπάρχουν αποτελέσματα αναζήτησης περιεχομένου
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 9f2c0273762f1a4a2b905487f461dc1d05db9209
ms.sourcegitcommit: 8f97342d8b46ab05f1e89018473caad9d35431df
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 07/19/2019
ms.locfileid: "35800362"
---
# <a name="no-results-from-content-searchexports"></a>Δεν υπάρχουν αποτελέσματα από περιεχομένου αναζήτησης-ΕΞΑΓΩΓΕΣ

Ζητήματα με περιεχομένου αναζήτησης/εξαγωγές δεν επιστρέφει δεδομένα ίσως οφείλεται σε ορισμένες φίλτρο ασφαλείας συμμόρφωσης που ήταν εγκατάστασης (Setup) από μια συγκεκριμένη Admin και δεν ανακοινώνουν όλα "διαχειριστές".

Για να επιλύσετε αυτό το πρόβλημα, ελέγξτε για να δείτε εάν υπάρχουν φίλτρα ασφαλείας συμμόρφωσης που μπορεί να προκαλούν αυτό:
1. Συνδεθείτε με ασφάλεια και Powershell συμμόρφωση παραγωγής
2. Εκτελέστε τις ακόλουθες commandlets:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter-$org την εταιρεία