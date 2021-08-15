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
ms.openlocfilehash: b134c952e3cc5305d8f3e6f44031e7f33d7938b67ff122c46cb74bbd33cbf59e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53994865"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Ορισμός του ClientAccessServerEnabled σε True

Εάν δεν μπορείτε να ανοίξετε ένα κρυπτογραφημένο μήνυμα ηλεκτρονικού ταχυδρομείου και αντί για αυτό δείτε ένα **συνημμένο rpmsg,** εκτελέστε τα παρακάτω βήματα:

1. Σύνδεση να Exchange Online PowerShell.

> [!NOTE]
> Για να συνδεθείτε Exchange Online PowerShell, πρέπει να εισέλθετε χρησιμοποιώντας έναν καθολικό διαχειριστή ή Exchange λογαριασμό διαχειριστή.

   a. Ανοίξτε Windows PowerShell και, στη συνέχεια, εκτελέστε την ακόλουθη εντολή:`$UserCredential = Get-Credential`
b. Στο παράθυρο **διαλόγου Windows PowerShell αίτηση διαπιστευτηρίων,** πληκτρολογήστε τον λογαριασμό και τον κωδικό πρόσβασης για τον σχολικό ή τον σχολικό λογαριασμό σας, γ. Κάντε κλικ στο κουμπί **OK**. 

2. Εκτελέστε την ακόλουθη εντολή για να δημιουργήσετε μια νέα περίοδο λειτουργίας:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. Εκτελέστε την παρακάτω εντολή:
    
    `Import-PSSession $Session -DisableNameChecking`

3. Εντολή `Get-IRMConfiguration` "Εκτέλεση".

4. Ελέγξτε τη **ρύθμιση ClientAccessServerEnabled.** 

    a. Εάν **η ρύθμιση ClientAccessServerEnabled** έχει οριστεί σε **False,** εκτελέστε το ακόλουθο cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

> [!TIP]
> Να κλείνετε πάντα την περίοδο λειτουργίας powershell με την ακόλουθη εντολή: `Remove-PSSession $Session`

Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

