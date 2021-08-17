---
title: Προβλήματα με την κατάργηση μιας συσκευής εκτός πίνακα ή μιας συσκευής που έχει απενεργοποιηθεί από το Απόθεμα συσκευών
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002913"
- "11187"
ms.openlocfilehash: 6eb59d16a1dab2de0e7a44faf9b34be6432342f9e20c94b6932e69e937751add
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57892003"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a>Προβλήματα με την κατάργηση μιας συσκευής εκτός πίνακα ή μιας συσκευής που έχει απενεργοποιηθεί από το Απόθεμα συσκευών

Προς το παρόν, ο Microsoft Defender για τελικό σημείο δεν επιτρέπει τη μη αυτόματη κατάργηση της εγγραφής συσκευής μιας συσκευής εκτός πίνακα ή μιας συσκευής που έχει απενεργοποιηθεί από το απόθεμα συσκευών.

Για λόγους ασφαλείας, η συσκευή παραμένει στην πύλη ως ιστορικό αρχείο για έως και 180 ημέρες. Ωστόσο, τα δεδομένα της συσκευής εκκαθαρισμένο σύμφωνα με τη ρυθμισμένη περίοδο διατήρησης.

**Σημείωση:** Μια συσκευή χωρίς πίνακα ή συσκευή εκτός λειτουργίας μεταβαίνει αυτόματα σε **κατάσταση αδράνειας** μετά από επτά ημέρες. Επιπλέον, οι συσκευές που δεν είναι ενεργές τις τελευταίες 30 ημέρες δεν λαμβάνονται υπόψη στα δεδομένα που απεικονίζουν τη βαθμολογία έκθεσης του οργανισμού Διαχείριση απειλών και ευπαθειών ή τη Βαθμολογία ασφαλείας της Microsoft για συσκευές.
 
Εάν εξακολουθείτε να μην θέλετε να βλέπετε συγκεκριμένες συσκευές στην προβολή "Απόθεμα συσκευών", δοκιμάστε να τοποθετήσετε μια ετικέτα συσκευής για να φιλτράρετε τη συσκευή που έχει τεθεί εκτός λειτουργίας από την προβολή "Απόθεμα συσκευών".

Για περισσότερες πληροφορίες, ανατρέξτε στα θέματα:

[Συσκευές offboard από την υπηρεσία Microsoft Defender για τελικά σημεία](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/offboard-machines.md)

[Βαθμολογία έκθεσης σε Διαχείριση απειλών και ευπαθειών](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[Επιδιόρθωση ανθυγιεινών αισθητήρων στο Microsoft Defender για το τελικό σημείο](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[Τρόπος αποτελεσματικής χρήσης της προσθήκης ετικετών (Μέρος 1)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[Τρόπος αποτελεσματικής χρήσης της προσθήκης ετικετών (Μέρος 2)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[Τρόπος αποτελεσματικής χρήσης της προσθήκης ετικετών (Μέρος 3)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




