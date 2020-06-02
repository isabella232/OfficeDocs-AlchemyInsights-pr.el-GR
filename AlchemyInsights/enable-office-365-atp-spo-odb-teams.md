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
ms.openlocfilehash: 564a7f1f6a37e64dbd7d679878ebadbbe35f3fa0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506918"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Ενεργοποίηση της Προηγμένης προστασίας από απειλές του Office 365 για ομάδες του SharePoint Online, του OneDrive και της Microsoft

1. Πήγαινε https://protection.office.com και συνδεθείτε.
2. Επιλέξτε **Ασφαλή**  >  συνημμένα**πολιτικής**  >  **διαχείρισης**απειλών .
3. Επιλέξτε **Ενεργοποίηση atp για ομάδες SharePoint, OneDrive και Microsoft**και, στη συνέχεια, κάντε κλικ στην επιλογή **Αποθήκευση**.
4. (Συνιστάται) Ως καθολικός διαχειριστής ή διαχειριστής του SharePoint Online, εκτελέστε το cmdlet [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) με την παράμετρο **DisallowInfectedFileDownload** που έχει οριστεί σε *true*.
5. (Συνιστάται) [Ρύθμιση ειδοποιήσεων](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) για αρχεία που εντοπίστηκαν.

> [!NOTE]
> Η ATP θα σαρώσει κάθε αρχείο στο SharePoint Online, το OneDrive ή το Microsoft Teams. Τα αρχεία σαρώνονται ασύγχρονα, μέσω μιας διαδικασίας που χρησιμοποιεί συμβάντα κοινής χρήσης και δραστηριότητας επισκεπτών, μαζί με έξυπνα ευρετική και σήματα απειλής για τον εντοπισμό κακόβουλων αρχείων. Ανατρέξτε [στο θέμα ATP για ομάδες του SharePoint, του OneDrive και του Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).