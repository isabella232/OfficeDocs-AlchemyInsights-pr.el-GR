---
title: Ενεργοποίηση Office 365 ATP για SharePoint, OneDrive και ομάδες της Microsoft
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: ae2f574663ae3233a056589c2d5a578171f3b2f4
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32403033"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Ενεργοποίηση Office 365 απειλή για προχωρημένους προστασίας για ηλεκτρονική SharePoint, OneDrive και ομάδες της Microsoft

1. Μεταβείτε στην https://protection.office.com και να εισέλθετε.
2. Επιλέξτε **Διαχείριση απειλή** > **πολιτική** > **Ασφαλή συνημμένα**.
3. Επιλέξτε **Ενεργοποίηση αυτόματης ασφάλειας Αμαξοστοιχίας για SharePoint, OneDrive, και ομάδες της Microsoft**και, στη συνέχεια, κάντε κλικ στο κουμπί **Αποθήκευση**.
4. (Συνιστάται) Ως ένας καθολικός διαχειριστής ή ένας διαχειριστής SharePoint Online, εκτελέστε το cmdlet [Σύνολο SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) με την παράμετρο **DisallowInfectedFileDownload** που έχει οριστεί στην *τιμή true*.
5. (Συνιστάται) [Ρύθμιση ειδοποιήσεων](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) για τα αρχεία που εντοπίστηκαν.

> [!NOTE]
> ATP θα nto σάρωση κάθε αρχείο σε ηλεκτρονική SharePoint, OneDrive ή ομάδες της Microsoft. Σάρωση των αρχείων γίνεται ασύγχρονα, μέσω μιας διαδικασίας που χρησιμοποιεί συμβάντα δραστηριότητα κοινής χρήσης και guest, καθώς και έξυπνες λύσεις και σήματα απειλή για τον προσδιορισμό κακόβουλα αρχεία. Ανατρέξτε στην ενότητα [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).