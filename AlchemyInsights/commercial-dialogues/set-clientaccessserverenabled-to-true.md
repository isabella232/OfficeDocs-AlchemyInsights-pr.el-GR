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
ms.openlocfilehash: fc953813a94c9ed3226f81f776d6085e12a6cafc
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320356"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Ορισμός του ClientAccessServerEnabled σε True

Εάν δεν μπορείτε να ανοίξετε ένα κρυπτογραφημένο μήνυμα ηλεκτρονικού ταχυδρομείου και αντί για αυτό δείτε ένα **συνημμένο rpmsg,** ακολουθήστε τα παρακάτω βήματα:

1. Σύνδεση στο Exchange Online PowerShell.

    **Σημείωση:** Για να συνδεθείτε Exchange Online PowerShell, πρέπει να εισέλθετε χρησιμοποιώντας έναν καθολικό διαχειριστή ή Exchange λογαριασμό διαχειριστή.

   a. Ανοίξτε Windows PowerShell και, στη συνέχεια, εκτελέστε την ακόλουθη εντολή:`$UserCredential = Get-Credential`
   b. Στο παράθυρο **διαλόγου Windows PowerShell αίτηση διαπιστευτηρίων,** πληκτρολογήστε τον λογαριασμό και τον κωδικό πρόσβασης για τον σχολικό ή τον σχολικό λογαριασμό σας, γ. Κάντε κλικ στο κουμπί **OK**. 

2. Εκτελέστε την ακόλουθη εντολή για να δημιουργήσετε μια νέα περίοδο λειτουργίας:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. Εκτελέστε την παρακάτω εντολή:
    
    `Import-PSSession $Session -DisableNameChecking`

3. Εντολή `Get-IRMConfiguration` "Εκτέλεση".

4. Ελέγξτε τη **ρύθμιση ClientAccessServerEnabled.** 

    a. Εάν **η ρύθμιση ClientAccessServerEnabled** έχει οριστεί σε **False,** εκτελέστε το ακόλουθο cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

**Συμβουλή:** Να κλείνετε πάντα την περίοδο λειτουργίας powershell με την ακόλουθη εντολή: `Remove-PSSession $Session`

Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

