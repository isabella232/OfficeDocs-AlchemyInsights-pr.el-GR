---
title: Κατάργηση της υπηρεσίας φόντου για την Αναζήτηση της Microsoft στο Bing
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816199"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a>Κατάργηση της υπηρεσίας φόντου για την Αναζήτηση της Microsoft στο Bing

Για να καταργήσετε την υπηρεσία φόντου για την Αναζήτηση της Microsoft στο Bing, μπορείτε να δοκιμάσετε τις ακόλουθες λύσεις:

1. Για να επιστρέψετε στις αρχικές ρυθμίσεις του μηχανισμού αναζήτησης, κάντε τα εξής:

    a. Απενεργοποιήστε **την επιλογή "Χρήση του Bing ως προεπιλεγμένου [μηχανισμού αναζήτησης".](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome)**

    b. [Μεταβείτε στο κέντρο διαχείρισης του Microsoft 365 και καταργήστε](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) τη ρύθμιση που επηρεάζει όλους τους χρήστες στον οργανισμό σας.

2. Για να καταργήσετε την υπηρεσία φόντου από μια μεμονωμένη συσκευή, κάντε τις ακόλουθες εργασίες:

    a. Επιλέξτε **"Πίνακας Ελέγχου" > "Προγράμματα" > "Προγράμματα και δυνατότητες".**

    b. Κάντε δεξί κλικ στην **Αναζήτηση της Microsoft στο Bing κάτω από τη** λίστα των εγκατεστημένων προγραμμάτων και, στη συνέχεια, κάντε κλικ στην επιλογή "Κατάργηση **εγκατάστασης".**

3. Για να καταργήσετε την υπηρεσία φόντου από πολλές συσκευές στον οργανισμό σας, συνδεθείτε ως διαχειριστής και εκτελέστε την ακόλουθη εντολή σε μια δέσμη ενεργειών: 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
