---
title: Ενεργοποίηση Θυρίδα συνημμένων για SharePoint Online, OneDrive και Microsoft Teams
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 61372075ac8ccf04606a8003b4ec29f89fc048e5
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332379"
---
# <a name="enable-safe-attachments-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Ενεργοποίηση Θυρίδα συνημμένων για SharePoint Online, OneDrive και Microsoft Teams

1. Χρησιμοποιώντας τα διαπιστευτήρια καθολικού διαχειριστή ή διαχειριστή ασφαλείας, ανοίξτε την πύλη Microsoft 365 Defender στην τοποθεσία και, στη συνέχεια, μεταβείτε στην ενότητα "Πολιτικές & κανόνες απειλών <https://security.microsoft.com>  \>  \> **Θυρίδα Συνημμένα"** στην ενότητα **"Πολιτικές"**

   Για να μεταβείτε απευθείας στη **Θυρίδα "Συνημμένα",** χρησιμοποιήστε <https://security.microsoft.com/safeattachmentv2> το .

2. Στη σελίδα **Θυρίδα συνημμένα, κάντε** κλικ στην επιλογή **"Καθολικές ρυθμίσεις".**
3. Στο αναδυόμενο στοιχείο που εμφανίζεται, επιλέξτε "Ενεργοποίηση του Microsoft Defender" για **Office 365 για SharePoint, OneDrive** και Microsoft Teams και, στη συνέχεια, επιλέξτε **"Αποθήκευση".**

    **Συμβουλή:** Ακολουθήστε τα παρακάτω βήματα για να βελτιώσετε την προστασία Θυρίδα συνημμένα για SharePoint, OneDrive και Microsoft Teams:
    - Για να αποτρέψετε τη λήψη κακόβουλων αρχείων από τους χρήστες, χρησιμοποιήστε την τιμή για την παράμετρο `$true` *DisallowInfectedFileDownload* στο **[cmdlet Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant)** στο SharePoint Online PowerShell. Για περισσότερες πληροφορίες, ανατρέξτε στο [θέμα SharePoint PowerShell online για να αποτρέψετε τη λήψη κακόβουλων αρχείων από τους χρήστες.](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-2-recommended-use-sharepoint-online-powershell-to-prevent-users-from-downloading-malicious-files)
    - [Δημιουργία πολιτικής ειδοποίησης για αρχεία που εντοπίστηκαν](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-3-recommended-use-the-microsoft-365-defender-portal-to-create-an-alert-policy-for-detected-files)

Για περισσότερες πληροφορίες, [ανατρέξτε Θυρίδα συνημμένα για Office 365 για SharePoint, OneDrive και Microsoft Teams.](https://go.microsoft.com/fwlink/?linkid=2092041)
