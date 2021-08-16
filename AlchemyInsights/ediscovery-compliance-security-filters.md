---
title: Δεν επιστρέφονται αποτελέσματα κατά την αναζήτηση/εξαγωγή περιεχομένου
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7463"
ms.openlocfilehash: 5c04364f98dccbcad0f011df866f137d79c166ad3839b408d6be447d50a87ac3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101266"
---
# <a name="no-results-returned-during-content-searchexport"></a>Δεν επιστρέφονται αποτελέσματα κατά την αναζήτηση/εξαγωγή περιεχομένου

Εάν αντιμετωπίζετε προβλήματα με τα ακόλουθα σενάρια eDiscovery:

- Η αναζήτηση/εξαγωγή περιεχομένου δεν επιστρέφει δεδομένα ή μη αναμενόμενα δεδομένα
- Η αναζήτηση ή η εξαγωγή eDiscovery αποτυγχάνει

Αυτό μπορεί να οφείλεται σε ορισμένα φίλτρα ασφάλειας συμμόρφωσης που έχουν μορφιστεί από έναν συγκεκριμένο διαχειριστή και δεν έχουν ανακοινωθεί σε όλους τους διαχειριστές.

Για να επιλύσετε αυτό το πρόβλημα, ελέγξτε εάν υπάρχουν φίλτρα ασφαλείας συμμόρφωσης που μπορεί να προκαλούν αυτά τα προβλήματα:

1. Σύνδεση στο Κέντρο ασφάλειας και συμμόρφωσης Powershell
2. Εκτελέστε τα ακόλουθα commandlet:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

Για πρόσθετες πληροφορίες σχετικά με τα φίλτρα ασφαλείας συμμόρφωσης, ανατρέξτε στο [θέμα "Φιλτράρισμα δικαιωμάτων για αναζήτηση περιεχομένου"](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
