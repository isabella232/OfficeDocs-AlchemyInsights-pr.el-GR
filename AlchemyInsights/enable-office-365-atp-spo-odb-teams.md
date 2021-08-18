---
title: Ενεργοποίηση Office 365 ATP για SharePoint, OneDrive και Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 2d132101768e0a835d448604d684ec0c735e6628
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332159"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Ενεργοποίηση του Microsoft Defender για Office 365 για SharePoint Online, OneDrive και Microsoft Teams

1. Μεταβείτε https://protection.office.com και πραγματοποιήστε είσοδο.
2. Επιλέξτε **Πολιτική διαχείρισης**  >  **απειλών**  >  **Θυρίδα συνημμένα.**
3. Επιλέξτε **"Ενεργοποίηση του Defender" για Office 365 για SharePoint, OneDrive και Microsoft Teams και, στη** συνέχεια, κάντε κλικ στην επιλογή **"Αποθήκευση".**
4. (Συνιστάται) Ως καθολικός διαχειριστής ή διαχειριστής του SharePoint Online, εκτελέστε το [cmdlet Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) με την παράμετρο **DisallowInfectedFileDownload** να έχει οριστεί σε *true.*
5. (Συνιστάται) [Ρύθμιση ειδοποιήσεων για](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) αρχεία που εντοπίστηκαν.

**Σημείωση:** Ο Microsoft Defender Office 365 δεν θα σαρώνει κάθε αρχείο SharePoint Online, OneDrive ή Microsoft Teams. Τα αρχεία σαρώνονται ασύγχρονα, μέσω μιας διαδικασίας που χρησιμοποιεί συμβάντα κοινής χρήσης και δραστηριότητας επισκεπτών, καθώς και έξυπνα heuristics και σήματα απειλών για τον προσδιορισμό κακόβουλων αρχείων. Ανατρέξτε [στο θέμα Microsoft Defender Office 365 για SharePoint, OneDrive και Microsoft Teams.](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)
