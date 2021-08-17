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
ms.openlocfilehash: b53534dd0666fa64e692910aa6800abab30169a97fbe567c815ce6b948381a63
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058002"
---
# <a name="no-results-from-content-searchexports"></a>Δεν υπάρχουν αποτελέσματα από την αναζήτηση/εξαγωγή περιεχομένου

Τα προβλήματα με την αναζήτηση περιεχομένου/τις εξαγωγές που δεν επιστρέφουν δεδομένα μπορεί να οφείλονται σε συγκεκριμένο φίλτρο ασφάλειας συμμόρφωσης που έχει μορφηθεί από έναν συγκεκριμένο διαχειριστή και δεν τα επικοινωνεί με όλους τους διαχειριστές.

Για να επιλύσετε αυτό το πρόβλημα, ελέγξτε εάν υπάρχουν φίλτρα ασφαλείας συμμόρφωσης που μπορεί να προκαλούν το εξής:
1. Σύνδεση στο Κέντρο ασφάλειας και συμμόρφωσης Powershell
2. Εκτελέστε τα ακόλουθα commandlet:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter -Οργάνωση $org