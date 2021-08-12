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
ms.openlocfilehash: 61ca448ef146f3f6fb930f0dc6f09f41bde72087f56ffba820f0a2d517cddb31
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53964633"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Ενεργοποίηση του Microsoft Defender για Office 365 για SharePoint Online, OneDrive και Microsoft Teams

1. Μεταβείτε https://protection.office.com και πραγματοποιήστε είσοδο.
2. Επιλέξτε **Πολιτική διαχείρισης**  >  **απειλών**  >  **Θυρίδα συνημμένα.**
3. Επιλέξτε **"Ενεργοποίηση του Defender" για Office 365 για SharePoint, OneDrive και Microsoft Teams και, στη** συνέχεια, κάντε κλικ στην επιλογή **"Αποθήκευση".**
4. (Συνιστάται) Ως καθολικός διαχειριστής ή διαχειριστής του SharePoint Online, εκτελέστε το [cmdlet Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) με την παράμετρο **DisallowInfectedFileDownload** να έχει οριστεί σε *true.*
5. (Συνιστάται) [Ρύθμιση ειδοποιήσεων για](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) αρχεία που εντοπίστηκαν.

> [!NOTE]
> Ο Microsoft Defender Office 365 δεν θα σαρώνει κάθε αρχείο SharePoint online, OneDrive ή Microsoft Teams. Τα αρχεία σαρώνονται ασύγχρονα, μέσω μιας διαδικασίας που χρησιμοποιεί συμβάντα κοινής χρήσης και δραστηριότητας επισκεπτών, καθώς και έξυπνα heuristics και σήματα απειλών για τον προσδιορισμό κακόβουλων αρχείων. Ανατρέξτε [στο θέμα Microsoft Defender για Office 365 για SharePoint, OneDrive και Microsoft Teams.](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)