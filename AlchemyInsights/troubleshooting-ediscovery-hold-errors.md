---
title: Η αντιμετώπιση προβλημάτων του ediscovery περιέχει σφάλματα
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 1df2b7153cac99419adc4f72b1c3732e7c746eac
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 05/20/2021
ms.locfileid: "52676149"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a>Η αντιμετώπιση προβλημάτων του ediscovery περιέχει σφάλματα

Αντιμετωπίζετε προβλήματα με τις κάτοχοι του eDiscovery; Ακολουθούν ορισμένες βέλτιστες πρακτικές που πρέπει να λάβετε υπόψη:

- Ελέγξτε την κατάσταση διανομής αναμονής.  Εάν η κατάσταση είναι **"Σε εκκρεμότητα"** ή **"Απενεργοποιημένη" (Σε εκκρεμότητα),** περιμένετε να ολοκληρωθεί η διανομή αναμονής.
- Συγχώνευση eDiscovery κρατήστε τις ενημερώσεις σε μια μεμονωμένη μαζική αίτηση αντί να ενημερώνετε την πολιτική επανειλημμένα για κάθε συναλλαγή.
- Εκτελέστε Set-CaseHoldPolicy <policyname> -RetryDistribution στο Powershell του Κέντρου ασφάλειας και συμμόρφωσης. Για λεπτομέρειες, ανατρέξτε [Σύνδεση στο Κέντρο ασφάλειας & PowerShell.](/powershell/exchange/connect-to-scc-powershell)

Για τα βήματα για να ελέγξετε αυτές τις ρυθμίσεις και πρόσθετες βέλτιστες πρακτικές για την αντιμετώπιση και την επίλυση προβλημάτων που περιέχει το eDiscovery, ανατρέξτε στο θέμα Αντιμετώπιση σφαλμάτων διατήρησης [του eDiscovery.](/microsoft-365/compliance/hold-distribution-errors)
Για πληροφορίες σχετικά με την αντιμετώπιση άλλων συνηθισμένων ζητημάτων eDiscovery, ανατρέξτε στο θέμα Διερεύνηση, αντιμετώπιση προβλημάτων και [επίλυση κοινών ζητημάτων eDiscovery.](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues)
