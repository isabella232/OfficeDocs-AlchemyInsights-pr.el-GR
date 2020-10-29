---
title: Ενεργοποίηση του Office 365 ATP για το SharePoint, το OneDrive και το Microsoft teams
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
ms.openlocfilehash: bef43656097c6f27677172899df1ada7900a9b64
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801048"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Ενεργοποίηση του Microsoft Defender για το Office 365 για το SharePoint Online, το OneDrive και το Microsoft teams

1. Μεταβείτε https://protection.office.com και πραγματοποιήστε είσοδο.
2. Επιλέξτε **Threat management**  >  **Policy**  >  **ασφαλή συνημμένα** πολιτικής διαχείρισης απειλών.
3. Επιλέξτε **Ενεργοποίηση ATP για το SharePoint, το OneDrive και το Microsoft teams** και, στη συνέχεια, κάντε κλικ στην επιλογή **Αποθήκευση** .
4. Συνιστάται Ως καθολικός διαχειριστής ή διαχειριστής του SharePoint Online, εκτελέστε το cmdlet [συνόλου-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) με την παράμετρο **DisallowInfectedFileDownload** ρυθμισμένη στην *τιμή TRUE* .
5. Συνιστάται [Ρύθμιση ειδοποιήσεων](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) για αρχεία που έχουν εντοπιστεί.

> [!NOTE]
> Το ATP δεν θα σαρώσει όλα τα αρχεία στο SharePoint Online, το OneDrive ή το Microsoft teams. Τα αρχεία σαρώνονται ασύγχρονα, μέσω μιας διαδικασίας που χρησιμοποιεί συμβάντα δραστηριοτήτων κοινής χρήσης και δραστηριοτήτων επισκεπτών, μαζί με έξυπνα ευρετικά στοιχεία και σήματα απειλών για τον εντοπισμό κακόβουλων αρχείων. Ανατρέξτε στο θέμα [ATP για SharePoint, OneDrive και Microsoft teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).