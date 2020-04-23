---
title: 932 Αναβάθμιση AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: fcc5fddb5cfd15407d0533449035317d187931ed
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766493"
---
# <a name="upgrade-azure-ad-connect"></a>Αναβάθμιση σύνδεσης azure ad

Από προεπιλογή, η αυτόματη αναβάθμιση είναι ενεργοποιημένη για το Azure AD Connect, το οποίο σας βοηθά να εξασφαλίσετε ότι εκτελείτε την πιο πρόσφατη έκδοση. Για να επαληθεύσετε τις ρυθμίσεις αυτόματης αναβάθμισης, χρησιμοποιήστε το cmdlet **Get-ADSyncAutoUpgrade** στο Azure AD PowerShell. Το cmdlet θα επιστρέψει μία από τις ακόλουθες τιμές:

- **Ενεργοποιημένο:** Η αυτόματη αναβάθμιση είναι ενεργοποιημένη.

- **Απενεργοποιημένο**: Η αυτόματη αναβάθμιση είναι απενεργοποιημένη.

- **Αναστολή:** Το σύστημα δεν είναι πλέον κατάλληλο για αυτόματη λήψη αναβαθμίσεων. Δεν μπορείτε να ρυθμίσετε αυτήν την τιμή. Έχει ρυθμιστεί από το σύστημα.

Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Αυτόματη αναβάθμιση](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Για να κάνετε λήψη της τελευταίας έκδοσης του Azure AD Connect, μεταβείτε στο [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).
