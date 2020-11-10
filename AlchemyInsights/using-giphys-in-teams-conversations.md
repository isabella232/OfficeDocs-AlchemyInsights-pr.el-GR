---
title: Χρήση του GIPHY σε συνομιλίες ομάδων
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
ms.openlocfilehash: 2fc29974bff9484c226c9651b9b000a89cad14dc
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982509"
---
# <a name="using-giphys-in-teams-conversations"></a>Χρήση του GIPHY σε συνομιλίες ομάδων

Η πρόσβαση GIPHY στη συνομιλία teams είναι ενεργοποιημένη από προεπιλογή. Ως διαχειριστής, μπορείτε να ελέγξετε εάν τα GIPHY είναι διαθέσιμα στους χρήστες Ορίζοντας [μια πολιτική ανταλλαγής μηνυμάτων](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) και εξασφαλίζοντας ότι η **χρήση του GIPHY στις συνομιλίες** είναι **ενεργοποιημένη**.

Εάν τα αρχεία GIF δεν λειτουργούν όπως αναμένεται στις συνομιλίες ομάδων, επαληθεύστε τα εξής:

Η [πολιτική ανταλλαγής μηνυμάτων](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) πρέπει να επιτρέπει το GIPHY. Για επαλήθευση με τη χρήση cmdlet PowerShell:

- Βεβαιωθείτε ότι μπορείτε να [διαχειριστείτε ομάδες με το PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).
- Εκτελέστε την εντολή PowerShell [Get-CsTeamsMessagingPolicy-Identity global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) και βεβαιωθείτε ότι το **AllowGiphy** έχει την τιμή **True**.
- Εάν το **AllowGiphy** έχει καθοριστεί σε **False** , εκτελέστε την ακόλουθη εντολή PowerShell- [CsTeamsMessagingPolicy-ταυτότητα global-AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

Οι [προαιρετικές συνδεδεμένες εμπειρίες](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) πρέπει να είναι ενεργοποιημένες για να επιτρέπουν την πρόσβαση στη διεύθυνση URL του GIPHY.

> [!NOTE]
> Εάν έχετε ρυθμίσει πολλές πολιτικές ανταλλαγής μηνυμάτων ομάδων για τον μισθωτή σας, μπορείτε να προσδιορίσετε την ταυτότητα της πολιτικής που έχει εκχωρηθεί στον χρήστη με την εντολή PowerShell [Get-CsOnlineUser-Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Επιλέξτε TeamsMessagingPolicy.
