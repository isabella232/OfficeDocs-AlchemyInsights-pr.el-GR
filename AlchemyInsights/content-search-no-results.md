---
title: Αναζήτηση περιεχομένου χωρίς αποτελέσματα
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 0267286ca5967ee891e65343d49adf776f0322a6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816848"
---
# <a name="no-results-from-content-searchexports"></a>Δεν υπάρχουν αποτελέσματα από την αναζήτηση/εξαγωγή περιεχομένου

Τα προβλήματα με την αναζήτηση περιεχομένου/τις εξαγωγές που δεν επιστρέφουν δεδομένα μπορεί να οφείλονται σε συγκεκριμένο φίλτρο ασφάλειας συμμόρφωσης που έχει μορφηθεί από έναν συγκεκριμένο διαχειριστή και δεν τα επικοινωνεί με όλους τους διαχειριστές.

Για να επιλύσετε αυτό το πρόβλημα, ελέγξτε εάν υπάρχουν φίλτρα ασφαλείας συμμόρφωσης που μπορεί να προκαλούν το εξής:
1. Σύνδεση στο Κέντρο ασφάλειας και συμμόρφωσης Powershell
2. Εκτελέστε τα ακόλουθα commandlet:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter -Οργάνωση $org