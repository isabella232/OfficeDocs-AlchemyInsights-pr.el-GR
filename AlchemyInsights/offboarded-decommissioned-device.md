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
ms.openlocfilehash: 814301e9cd8197e62dcca68ab3bdde1618d210f73a744b53bb5af7b861eb02bf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54076652"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a>Προβλήματα με την κατάργηση μιας συσκευής εκτός πίνακα ή μιας συσκευής που έχει απενεργοποιηθεί από το Απόθεμα συσκευών

Προς το παρόν, ο Microsoft Defender για τελικό σημείο δεν επιτρέπει τη μη αυτόματη κατάργηση της εγγραφής συσκευής μιας συσκευής εκτός πίνακα ή μιας συσκευής που έχει απενεργοποιηθεί από το απόθεμα συσκευών.

Για λόγους ασφαλείας, η συσκευή παραμένει στην πύλη ως ιστορικό αρχείο για έως και 180 ημέρες. Ωστόσο, τα δεδομένα της συσκευής εκκαθαρίστηκε σύμφωνα με τη ρυθμισμένη περίοδο διατήρησης.

**Σημείωση:** Μια συσκευή χωρίς πίνακα ή συσκευή εκτός λειτουργίας μεταβαίνει αυτόματα σε **κατάσταση αδράνειας** μετά από επτά ημέρες. Επιπλέον, οι συσκευές που δεν είναι ενεργές τις τελευταίες 30 ημέρες δεν λαμβάνονται υπόψη στα δεδομένα που απεικονίζουν τη βαθμολογία Διαχείριση απειλών και ευπαθειών έκθεσης του οργανισμού σας ή τη Βαθμολογία ασφαλείας της Microsoft για συσκευές.
 
Εάν εξακολουθείτε να μην θέλετε να βλέπετε συγκεκριμένες συσκευές στην προβολή "Απόθεμα συσκευών", δοκιμάστε να τοποθετήσετε μια ετικέτα συσκευής για να φιλτράρετε τη συσκευή που έχει τεθεί εκτός λειτουργίας από την προβολή "Απόθεμα συσκευών".

Για περισσότερες πληροφορίες, ανατρέξτε στα θέματα:

[Συσκευές offboard από την υπηρεσία Microsoft Defender για τελικά σημεία](/microsoft-365/security/defender-endpoint/offboard-machines.md)

[Βαθμολογία έκθεσης σε Διαχείριση απειλών και ευπαθειών](/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[Επιδιόρθωση ανθυγιεινών αισθητήρων στο Microsoft Defender για το τελικό σημείο](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[Τρόπος αποτελεσματικής χρήσης της προσθήκης ετικετών (Μέρος 1)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[Τρόπος αποτελεσματικής χρήσης της προσθήκης ετικετών (Μέρος 2)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[Τρόπος αποτελεσματικής χρήσης της προσθήκης ετικετών (Μέρος 3)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




