---
title: Πραγματοποιήστε είσοδο στο Microsoft Edge με μη αυτόματο τρόπο
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
ms.openlocfilehash: c5d71c26ba3584f8ce496a28587fe75cae2d344f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677790"
---
# <a name="sign-in-to-microsoft-edge-manually"></a>Πραγματοποιήστε είσοδο στο Microsoft Edge με μη αυτόματο τρόπο

Εάν ένας χρήστης δεν εισέλθει αυτόματα κατά τη διάρκεια μιας εμπειρίας πρώτης εκτέλεσης, ο χρήστης μπορεί να πραγματοποιήσει είσοδο με μη αυτόματο τρόπο μέσω των ρυθμίσεων του προγράμματος περιήγησης ή του αναδυόμενου στοιχείου ταυτότητας. Για να διαχειριστείτε τη σύνδεση, χρησιμοποιήστε τις ακόλουθες πολιτικές:

1. [NonRemovableProfileEnabled](https://docs.microsoft.com/deployedge/microsoft-edge-policies#nonremovableprofileenabled) -για να εξασφαλίσετε ότι ο χρήστης έχει πάντα ένα προφίλ εργασίας στο Microsoft Edge.
2. [RestrictSigninToPattern](https://docs.microsoft.com/deployedge/microsoft-edge-policies#restrictsignintopattern) -για να περιορίσετε την είσοδο σε ένα καθορισμένο μέρος αξιόπιστων λογαριασμών.
3. [BrowserSignin](https://docs.microsoft.com/deployedge/microsoft-edge-policies#browsersignin) -για να απενεργοποιήσετε την είσοδο ή για να αναγκάσετε τους χρήστες να πραγματοποιήσουν είσοδο.

