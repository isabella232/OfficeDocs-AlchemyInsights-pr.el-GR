---
title: Είσοδος στον Microsoft Edge με μη αυτόματο τρόπο
ms.author: v-smandalika
author: v-smandalika
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9003844"
- "6893"
- "8332"
- "9004625"
ms.openlocfilehash: f380d09dc14788205638cdee6aebe0b084ecab2f
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398657"
---
# <a name="sign-in-to-microsoft-edge-manually"></a>Είσοδος στον Microsoft Edge με μη αυτόματο τρόπο

Εάν ένας χρήστης δεν έχει εισέλθει αυτόματα κατά τη διάρκεια μιας εμπειρίας πρώτης εκτέλεσης, ο χρήστης μπορεί να συνδεθεί με μη αυτόματο τρόπο μέσω των ρυθμίσεων του προγράμματος περιήγησης ή του αναδυόμενου ορίου ταυτότητας. Για να διαχειριστείτε την είσοδο, χρησιμοποιήστε τις ακόλουθες πολιτικές:

1. [NonRemovableProfileEnabled](https://docs.microsoft.com/deployedge/microsoft-edge-policies#nonremovableprofileenabled) - Για να βεβαιωθείτε ότι ένας χρήστης έχει πάντα ένα προφίλ εργασίας στον Microsoft Edge.
2. [RestrictSigninToPattern](https://docs.microsoft.com/deployedge/microsoft-edge-policies#restrictsignintopattern) - Για να περιορίσετε την είσοδο σε ένα σύνολο αξιόπιστων λογαριασμών.
3. [BrowserSignin](https://docs.microsoft.com/deployedge/microsoft-edge-policies#browsersignin) - Για να απενεργοποιήσετε την είσοδο ή για να επιβάλετε στους χρήστες να πραγματοποιήσουν είσοδο.

