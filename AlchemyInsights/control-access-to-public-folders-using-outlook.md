---
title: Έλεγχος της πρόσβασης σε δημόσιους φακέλους με χρήση Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 1386b97f804e63455094abf64b9d9e2541d57dafa36535813b0d7689e0ce2966
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54032558"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Έλεγχος της πρόσβασης σε δημόσιους φακέλους με χρήση Outlook

Για να ελέγξετε ποιοι χρήστες μπορούν να αποκτήσουν πρόσβαση σε δημόσιους φακέλους χρησιμοποιώντας Outlook:

1. Χρήση `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: Να επιτρέπεται στους χρήστες η πρόσβαση σε δημόσιους φακέλους Outlook  
$false: Αποτρέψτε την πρόσβαση των χρηστών σε δημόσιους φακέλους Outlook. Αυτή είναι η προεπιλεγμένη τιμή.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Σημείωση: Αυτή η διαδικασία μπορεί να ελέγξει μόνο τις συνδέσεις με Outlook υπολογιστή για Windows υπολογιστές-πελάτες. Οι χρήστες μπορούν να συνεχίσουν να έχουν πρόσβαση σε δημόσιους φακέλους χρησιμοποιώντας το OWA ή Outlook για Mac.

Για περισσότερες πληροφορίες, ανατρέξτε στο [θέμα Ελεγχόμενες συνδέσεις σε δημόσιους φακέλους Outlook](https://aka.ms/controlpf) για περισσότερες πληροφορίες.
