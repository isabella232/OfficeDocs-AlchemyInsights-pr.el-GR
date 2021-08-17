---
title: 932 Αναβάθμιση AADConnect
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
ms.openlocfilehash: 9582f1f56e6730e35520b5d79bc245cd74bea0bf4db39b379a7cd133bafc16ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104812"
---
# <a name="upgrade-azure-ad-connect"></a>Αναβάθμιση του Azure AD Σύνδεση

Από προεπιλογή, η αυτόματη αναβάθμιση είναι ενεργοποιημένη για το Azure AD Σύνδεση, γεγονός που σας βοηθά να εξασφαλίσετε ότι χρησιμοποιείτε την πιο πρόσφατη έκδοση. Για να επαληθεύσετε τις ρυθμίσεις αυτόματης αναβάθμισης, χρησιμοποιήστε το **cmdlet Get-ADSyncAutoUpgrade** στο Azure AD PowerShell. Το cmdlet θα επιστρέψει μία από τις παρακάτω τιμές:

- **Ενεργοποιημένο:** Η αυτόματη αναβάθμιση είναι ενεργοποιημένη.

- **Απενεργοποιημένο:** Η αυτόματη αναβάθμιση είναι απενεργοποιημένη.

- **Σε αναστολή:** Το σύστημα δεν είναι πλέον κατάλληλο για τη λήψη αυτόματων αναβαθμίσεων. Δεν μπορείτε να ρυθμίσετε τις παραμέτρους αυτής της τιμής. ορίζεται από το σύστημα.

Για περισσότερες πληροφορίες, ανατρέξτε στο [θέμα Αυτόματη αναβάθμιση.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)

Για να κάνετε λήψη της πιο πρόσφατης έκδοσης του Azure AD Σύνδεση, μεταβείτε στο [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .
