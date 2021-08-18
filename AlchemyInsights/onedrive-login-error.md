---
title: OneDrive σφάλματος σύνδεσης AADSTS50011
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003820"
- "6840"
ms.openlocfilehash: 80aafa2aee7213e1b77d274509a7eb9741c20b525ed97f473093ac8c6514f3c7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54112912"
---
# <a name="onedrive-login-error-aadsts50011"></a>OneDrive σφάλματος σύνδεσης AADSTS50011

Εάν εμφανιστεί το σφάλμα "AADSTS50011: Η διεύθυνση URL απάντησης που καθορίζεται στην αίτηση δεν συμφωνεί με την απάντηση" κατά την είσοδο στην εφαρμογή OneDrive, ελέγξτε για τα εξής:

Η OneDrive έκδοση πρέπει να είναι ίση ή μεγαλύτερη από την έκδοση 20.052.XXXX.XXXX. Για να ελέγξετε την έκδοση, κάντε κλικ στο μπλε OneDrive στην περιοχή ειδοποιήσεων, επιλέξτε **"Βοήθεια" & Ρυθμίσεις > Ρυθμίσεις > Πληροφορίες.**

Το δίκτυό σας ενδέχεται να αποκλείσει **την κυκλοφορία g.live.com** και **oneclient.sfx.ms.** Εάν αυτή η κυκλοφορία έχει αποκλειστεί, OneDrive να ενημερωθεί. Συνεργαστείτε με το διαχειριστή του δικτύου σας για να βεβαιωθείτε ότι έχετε πρόσβαση σε αυτές τις διευθύνσεις URL. [Αυτά τα τελικά σημεία θα πρέπει](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) να είναι προσιτά για τους πελάτες που χρησιμοποιούν Microsoft 365 προγραμμάτων.

Εάν θέλετε να λάβετε με μη αυτόματο τρόπο μια τρέχουσα έκδοση του OneDrive, επισκεφθείτε την τοποθεσία [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .
