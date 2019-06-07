---
title: 932 AADConnect αναβάθμιση
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 932
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 210f230929db72027a0f729b17901fe88eb45709
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34757291"
---
# <a name="upgrade-azure-ad-connect"></a>Αναβάθμιση Azure AD σύνδεση

Από προεπιλογή, ενεργοποιείται η Αυτόματη αναβάθμιση για σύνδεση AD Azure, που συμβάλλει ώστε να χρησιμοποιείτε την πιο πρόσφατη έκδοση. Για να επαληθεύσετε τις ρυθμίσεις αυτόματης αναβάθμισης, χρησιμοποιήστε το cmdlet **Get-ADSyncAutoUpgrade** σε Azure AD PowerShell. Το cmdlet θα επιστρέψει μία από τις ακόλουθες τιμές: 

- **Ενεργοποίηση**: Αυτόματη αναβάθμιση είναι ενεργοποιημένη.

- **Απενεργοποιημένο**: Αυτόματη αναβάθμιση είναι απενεργοποιημένη.

- **Αναστολής**: το σύστημα δεν είναι πλέον επιλέξιμες να λαμβάνετε αυτόματες αναβαθμίσεις. Δεν μπορείτε να ρυθμίσετε αυτήν την τιμή; ορίζεται από το σύστημα. 

Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Αυτόματη αναβάθμιση](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Για να κάνετε λήψη της τελευταίας έκδοσης του σύνδεση AD Azure, μεταβείτε στο [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).
