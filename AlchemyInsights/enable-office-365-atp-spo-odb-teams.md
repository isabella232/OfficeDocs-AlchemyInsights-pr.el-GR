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
ms.openlocfilehash: dd367176f8d6f38f1f94ae6627229234f15c81ff
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543928"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Ενεργοποίηση του Microsoft Defender για Office 365 για SharePoint Online, OneDrive και Microsoft Teams

1. Μεταβείτε https://protection.office.com και πραγματοποιήστε είσοδο.
2. Επιλέξτε **"Ασφαλή**  >  **συνημμένα πολιτικής** διαχείρισης  >  **απειλών".**
3. Επιλέξτε **"Ενεργοποίηση του Defender" για Office 365 για SharePoint, OneDrive και Microsoft Teams και, στη** συνέχεια, κάντε κλικ στην επιλογή **"Αποθήκευση".**
4. (Συνιστάται) Ως καθολικός διαχειριστής ή διαχειριστής του SharePoint Online, εκτελέστε το [cmdlet Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) με την παράμετρο **DisallowInfectedFileDownload** να έχει οριστεί σε *true.*
5. (Συνιστάται) [Ρύθμιση ειδοποιήσεων για](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) αρχεία που εντοπίστηκαν.

> [!NOTE]
> Ο Microsoft Defender Office 365 δεν θα σαρώνει κάθε αρχείο SharePoint online, OneDrive ή Microsoft Teams. Τα αρχεία σαρώνονται ασύγχρονα, μέσω μιας διαδικασίας που χρησιμοποιεί συμβάντα κοινής χρήσης και δραστηριότητας επισκεπτών, καθώς και έξυπνα heuristics και σήματα απειλών για τον προσδιορισμό κακόβουλων αρχείων. Ανατρέξτε [στο θέμα Microsoft Defender για Office 365 για SharePoint, OneDrive και Microsoft Teams.](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)