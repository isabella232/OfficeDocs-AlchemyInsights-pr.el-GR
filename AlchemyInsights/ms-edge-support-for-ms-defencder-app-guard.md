---
title: Υποστήριξη του Microsoft Edge για το προστατευτικό εφαρμογής του Microsoft Defender
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583584"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a>Υποστήριξη του Microsoft Edge για το προστατευτικό εφαρμογής του Microsoft Defender

Σχεδιασμένο για Windows 10 και Microsoft Edge, το Guard εφαρμογών χρησιμοποιεί μια προσέγγιση απομόνωσης υλικού, η οποία επιτρέπει στους χρήστες να περιηγηθούν σε μη αξιόπιστες τοποθεσίες μέσα σε ένα απομονωμένο κοντέινερ με δυνατότητα Hyper-V, το οποίο διαχωρίζεται από το λειτουργικό σύστημα του κεντρικού υπολογιστή.

Ένας διαχειριστής εταιρείας ορίζει μια λίστα αξιόπιστων τοποθεσιών Web, πόρων cloud και εσωτερικών δικτύων. Όταν ένας χρήστης επισκέπτεται μια τοποθεσία που δεν υπάρχει στη λίστα, το Microsoft Edge θα ανοίξει την τοποθεσία στο κοντέινερ. Αυτό σημαίνει ότι εάν η τοποθεσία αποδειχθεί κακόβουλη, ο κεντρικός ΥΠΟΛΟΓΙΣΤΉς θα παραμείνει προστατευμένος και ο εισβολέας δεν θα φτάσει στα εταιρικά δεδομένα.

Η εγκατάσταση των επεκτάσεων στο κοντέινερ υποστηρίζεται από το Microsoft Edge έκδοση 81 και μπορεί να ελεγχθεί μέσω μιας πολιτικής. Η διεύθυνση updateURL που χρησιμοποιείται στην πολιτική ExtensionInstallForcelist θα πρέπει να προστεθεί ως ουδέτερος πόρος στις πολιτικές απομόνωσης δικτύου που χρησιμοποιούνται από το Guard εφαρμογών.

Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [υποστήριξη του Microsoft Edge για το προστατευτικό εφαρμογής του Microsoft Defender](https://go.microsoft.com/fwlink/?linkid=2134229).
