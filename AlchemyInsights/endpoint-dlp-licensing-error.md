---
title: Σφάλμα παραχώρησης αδειών χρήσης DLP τελικού σημείου
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200001"
- "7176"
ms.openlocfilehash: 1e242abe18717e5ef64d6f067ab3ec6fa8833cb672dd21c85e577ce640240ba0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090140"
---
# <a name="endpoint-dlp-licensing-error"></a>Σφάλμα παραχώρησης αδειών χρήσης DLP τελικού σημείου

Όταν προσπαθείτε να ρυθμίσετε το DLP τελικού σημείου, εάν εμφανιστεί το ακόλουθο σφάλμα:

`Your organization is missing the licenses required to manage these devices`.

Βεβαιωθείτε ότι έχετε μία από τις ακόλουθες συνδρομές ή πρόσθετα:

- Microsoft 365 E5
- Microsoft 365 A5 (EDU)
- Microsoft 365 E5 συμμόρφωσης
- Microsoft 365 A5 συμμόρφωσης
- Microsoft 365 E5 προστασίας και διακυβέρνησης των πληροφοριών
- Microsoft 365 A5 προστασίας και διακυβέρνησης των πληροφοριών

> [!NOTE]
> Αυτό δεν θα λειτουργεί για συνδυασμούς αδειών χρήσης, όπως: Win E5 + O365 E5 + EMS E5. Για να ρυθμίσετε αυτήν τη δυνατότητα, πρέπει να έχετε μια καθαρή άδεια χρήσης M365 E5.

Για περισσότερες πληροφορίες παραχώρησης αδειών χρήσης DLP τελικού σημείου, ανατρέξτε στο [θέμα Άδειες χρήσης DLP τελικού σημείου.](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)
