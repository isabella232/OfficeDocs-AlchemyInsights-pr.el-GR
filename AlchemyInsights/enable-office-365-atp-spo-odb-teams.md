---
title: Ενεργοποίηση atp του Office 365 για ομάδες Του SharePoint, OneDrive και Microsoft
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: fdfdc97a198898051a3388672d01994d96dd5e97
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703426"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Ενεργοποίηση της Προηγμένης προστασίας από απειλές του Office 365 για ομάδες του SharePoint Online, του OneDrive και της Microsoft

1. Πήγαινε https://protection.office.com και συνδεθείτε.
2. Επιλέξτε**Ασφαλή συνημμένα****πολιτικής** >  **διαχείρισης** > απειλών .
3. Επιλέξτε **Ενεργοποίηση atp για ομάδες SharePoint, OneDrive και Microsoft**και, στη συνέχεια, κάντε κλικ στην επιλογή **Αποθήκευση**.
4. (Συνιστάται) Ως καθολικός διαχειριστής ή διαχειριστής του SharePoint Online, εκτελέστε το cmdlet [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) με την παράμετρο **DisallowInfectedFileDownload** που έχει οριστεί σε *true*.
5. (Συνιστάται) [Ρύθμιση ειδοποιήσεων](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) για αρχεία που εντοπίστηκαν.

> [!NOTE]
> Η ATP θα σαρώσει κάθε αρχείο στο SharePoint Online, το OneDrive ή το Microsoft Teams. Τα αρχεία σαρώνονται ασύγχρονα, μέσω μιας διαδικασίας που χρησιμοποιεί συμβάντα κοινής χρήσης και δραστηριότητας επισκεπτών, μαζί με έξυπνα ευρετική και σήματα απειλής για τον εντοπισμό κακόβουλων αρχείων. Βλέπε [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).