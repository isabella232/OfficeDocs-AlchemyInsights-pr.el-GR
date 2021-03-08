---
title: Ορισμός του ClientAccessServerEnabled σε True
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524557"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Ορισμός του ClientAccessServerEnabled σε True

Εάν δεν μπορείτε να ανοίξετε ένα κρυπτογραφημένο μήνυμα ηλεκτρονικού ταχυδρομείου και αντί για αυτό δείτε ένα **συνημμένο rpmsg,** εκτελέστε τα ακόλουθα βήματα:

1. Συνδεθείτε στο Exchange Online PowerShell.

> [!NOTE]
> Για να συνδεθείτε στο Exchange Online PowerShell, πρέπει να εισέλθετε χρησιμοποιώντας έναν καθολικό διαχειριστή ή ένα λογαριασμό διαχειριστή του Exchange.

   a. Ανοίξτε το Windows PowerShell και, στη συνέχεια, εκτελέστε την ακόλουθη εντολή: `$UserCredential = Get-Credential`
b. Στο παράθυρο διαλόγου **"Αίτηση διαπιστευτηρίων" του Windows PowerShell,** εισαγάγετε τον λογαριασμό εργασίας ή το σχολείο σας και τον κωδικό πρόσβασης, γ. Κάντε κλικ στο κουμπί **OK**. 

2. Εκτελέστε την ακόλουθη εντολή για να δημιουργήσετε μια νέα περίοδο λειτουργίας:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. Εκτελέστε την παρακάτω εντολή:
    
    `Import-PSSession $Session -DisableNameChecking`

3. Εντολή `Get-IRMConfiguration` "Εκτέλεση".

4. Ελέγξτε τη **ρύθμιση ClientAccessServerEnabled.** 

    a. Εάν **η ρύθμιση ClientAccessServerEnabled** έχει οριστεί σε **False,** εκτελέστε το ακόλουθο cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

> [!TIP]
> Κλείνετε πάντα την περίοδο λειτουργίας του PowerShell με την ακόλουθη εντολή: `Remove-PSSession $Session`

Για περισσότερες πληροφορίες, ανατρέξτε [στο Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

