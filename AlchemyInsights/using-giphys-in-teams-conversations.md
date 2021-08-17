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
ms.openlocfilehash: 0244b68ffa2ebd3d70bae66a24ac299004848557b63b17c2ea74fafaff22bb8c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104308"
---
# <a name="using-giphys-in-teams-conversations"></a>Χρήση giphy σε Teams συνομιλιών

Η πρόσβαση giphys Teams συνομιλίας είναι ενεργοποιημένη από προεπιλογή. Ως διαχειριστής, μπορείτε να ελέγξετε εάν το [](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) Giphy είναι διαθέσιμο στους χρήστες, ορίζοντας μια πολιτική ανταλλαγής μηνυμάτων και εξασφαλίζοντας ότι η **δυνατότητα "Χρήση Giphys σε συνομιλίες"** είναι **"Σε"**.

Εάν τα GIF δεν λειτουργούν όπως αναμένεται σε Teams συνομιλιών, επαληθεύστε:

Η [πολιτική ανταλλαγής μηνυμάτων πρέπει](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) να επιτρέπει giphy. Για να το επαληθεύσετε χρησιμοποιώντας cmdlet του PowerShell:

- Βεβαιωθείτε ότι μπορείτε να [διαχειριστείτε Teams το PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell)
- Εκτελέστε την εντολή PowerShell [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) και βεβαιωθείτε ότι **το AllowGiphy** έχει οριστεί σε **TRUE.**
- Εάν **το AllowGiphy** έχει οριστεί σε **FALSE,** εκτελέστε την ακόλουθη εντολή PowerShell [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True.](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps)

[Οι προαιρετικές συνδεδεμένες](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) εμπειρίες πρέπει να είναι ενεργοποιημένες για να επιτρέπεται η πρόσβαση στη διεύθυνση URL giphy.

> [!NOTE]
> Εάν έχετε ρυθμίσει πολλές πολιτικές ανταλλαγής Teams μηνυμάτων για το μισθωτή σας, μπορείτε να προσδιορίσετε την ταυτότητα της πολιτικής που έχει εκχωρηθεί στον χρήστη που έχει επιπτώσεις με την εντολή ["Λήψη CsOnlineUser- Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Επιλέξτε TeamsMessagingPolicy.
