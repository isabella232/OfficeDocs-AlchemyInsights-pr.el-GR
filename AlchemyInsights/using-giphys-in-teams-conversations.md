---
title: Χρήση giphy σε Teams συνομιλιών
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003825"
- "6850"
ms.openlocfilehash: 296c2f80d35f1c93ab3c60e0be65fd96c953ca81
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323520"
---
# <a name="using-giphys-in-teams-conversations"></a>Χρήση giphy σε Teams συνομιλιών

Η πρόσβαση giphys Teams συνομιλίας είναι ενεργοποιημένη από προεπιλογή. Ως διαχειριστής, μπορείτε να ελέγξετε εάν τα [](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) Giphy είναι διαθέσιμα στους χρήστες, ορίζοντας μια πολιτική ανταλλαγής μηνυμάτων και εξασφαλίζοντας ότι η **δυνατότητα "Χρήση Giphys" σε συνομιλίες** είναι **"Σε"**.

Εάν τα GIF δεν λειτουργούν όπως αναμένεται σε Teams συνομιλιών, επαληθεύστε:

Η [πολιτική ανταλλαγής μηνυμάτων](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) πρέπει να επιτρέπει giphy. Για να το επαληθεύσετε χρησιμοποιώντας cmdlet του PowerShell:

- Βεβαιωθείτε ότι μπορείτε να [διαχειριστείτε Teams το PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell)
- Εκτελέστε την εντολή PowerShell [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) και βεβαιωθείτε ότι **το AllowGiphy** έχει οριστεί σε **TRUE.**
- Εάν **το AllowGiphy** έχει οριστεί σε **FALSE,** εκτελέστε την ακόλουθη εντολή PowerShell [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True.](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps)

[Οι προαιρετικές συνδεδεμένες](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) εμπειρίες πρέπει να είναι ενεργοποιημένες για να επιτρέπεται η πρόσβαση στη διεύθυνση URL giphy.

**Σημείωση:** Εάν έχετε ρυθμίσει πολλές πολιτικές ανταλλαγής μηνυμάτων του Teams για το μισθωτή σας, μπορείτε να προσδιορίσετε την ταυτότητα της πολιτικής που έχει εκχωρηθεί στον χρήστη που έχει επιπτώσεις με την εντολή ["Get-CsOnlineUser-Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Επιλέξτε TeamsMessagingPolicy.
