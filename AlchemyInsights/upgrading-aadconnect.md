---
title: 932 αναβάθμιση AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 5c8ec5d9282c53c655e28f5d38fe36fc3ab005b8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806039"
---
# <a name="upgrade-azure-ad-connect"></a>Αναβάθμιση σύνδεσης Azure AD

Από προεπιλογή, η αυτόματη αναβάθμιση είναι ενεργοποιημένη για το Azure AD Connect, γεγονός που σας βοηθά να διασφαλίσετε ότι χρησιμοποιείτε την πιο πρόσφατη έκδοση. Για να επαληθεύσετε τις ρυθμίσεις αυτόματης αναβάθμισης, χρησιμοποιήστε το cmdlet **Get-ADSyncAutoUpgrade** στο Azure AD PowerShell. Το cmdlet θα επιστρέψει μία από τις ακόλουθες τιμές:

- **Ενεργοποιημένο**: η αυτόματη αναβάθμιση είναι ενεργοποιημένη.

- **Απενεργοποιημένη**: η αυτόματη αναβάθμιση είναι απενεργοποιημένη.

- **Αναστέλλεται**: το σύστημα δεν είναι πλέον επιλέξιμο για τη λήψη αυτόματων ενημερώσεων. Δεν μπορείτε να ρυθμίσετε τις παραμέτρους αυτής της τιμής. έχει καθοριστεί από το σύστημα.

Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Αυτόματη αναβάθμιση](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Για να κάνετε λήψη της πιο πρόσφατης έκδοσης του Azure AD Connect, μεταβείτε στο [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .
