---
title: Έλεγχος της πρόσβασης σε δημόσιους φακέλους με χρήση του Outlook
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
ms.openlocfilehash: f528044ca7f6f2ee2812f9f831093c44eca26fe1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816740"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Έλεγχος της πρόσβασης σε δημόσιους φακέλους με χρήση του Outlook

Για να ελέγξετε ποιοι χρήστες μπορούν να έχουν πρόσβαση σε δημόσιους φακέλους χρησιμοποιώντας το Outlook:

1. Χρήση `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: Να επιτρέπεται στους χρήστες η πρόσβαση σε δημόσιους φακέλους στο Outlook  
$false: Αποτρέψτε την πρόσβαση των χρηστών σε δημόσιους φακέλους στο Outlook. Αυτή είναι η προεπιλεγμένη τιμή.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Σημείωση: Αυτή η διαδικασία μπορεί να ελέγξει μόνο τις συνδέσεις με υπολογιστές-πελάτες του Outlook για Windows. Οι χρήστες μπορούν να συνεχίσουν να έχουν πρόσβαση σε δημόσιους φακέλους χρησιμοποιώντας το OWA ή το Outlook για Mac.

Για περισσότερες πληροφορίες, ανατρέξτε στο [θέμα Ελεγχόμενες συνδέσεις σε δημόσιους φακέλους στο Outlook](https://aka.ms/controlpf) για περισσότερες πληροφορίες.
