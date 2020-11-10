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
# <a name="using-giphys-in-teams-conversations"></a><span data-ttu-id="172c5-102">Χρήση του GIPHY σε συνομιλίες ομάδων</span><span class="sxs-lookup"><span data-stu-id="172c5-102">Using Giphys in Teams Conversations</span></span>

<span data-ttu-id="172c5-103">Η πρόσβαση GIPHY στη συνομιλία teams είναι ενεργοποιημένη από προεπιλογή.</span><span class="sxs-lookup"><span data-stu-id="172c5-103">Giphys access in Teams chat is enabled by default.</span></span> <span data-ttu-id="172c5-104">Ως διαχειριστής, μπορείτε να ελέγξετε εάν τα GIPHY είναι διαθέσιμα στους χρήστες Ορίζοντας [μια πολιτική ανταλλαγής μηνυμάτων](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) και εξασφαλίζοντας ότι η **χρήση του GIPHY στις συνομιλίες** είναι **ενεργοποιημένη**.</span><span class="sxs-lookup"><span data-stu-id="172c5-104">As an administrator, you can control if Giphys are available to users by [setting a messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) and ensuring that **Use Giphys in conversations** is **On**.</span></span>

<span data-ttu-id="172c5-105">Εάν τα αρχεία GIF δεν λειτουργούν όπως αναμένεται στις συνομιλίες ομάδων, επαληθεύστε τα εξής:</span><span class="sxs-lookup"><span data-stu-id="172c5-105">If GIFs are not working as expected in Teams conversations, verify:</span></span>

<span data-ttu-id="172c5-106">Η [πολιτική ανταλλαγής μηνυμάτων](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) πρέπει να επιτρέπει το GIPHY.</span><span class="sxs-lookup"><span data-stu-id="172c5-106">The [messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) needs to allow Giphys.</span></span> <span data-ttu-id="172c5-107">Για επαλήθευση με τη χρήση cmdlet PowerShell:</span><span class="sxs-lookup"><span data-stu-id="172c5-107">To verify by using PowerShell cmdlets:</span></span>

- <span data-ttu-id="172c5-108">Βεβαιωθείτε ότι μπορείτε να [διαχειριστείτε ομάδες με το PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span><span class="sxs-lookup"><span data-stu-id="172c5-108">Verify that you can [Manage Teams with PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span></span>
- <span data-ttu-id="172c5-109">Εκτελέστε την εντολή PowerShell [Get-CsTeamsMessagingPolicy-Identity global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) και βεβαιωθείτε ότι το **AllowGiphy** έχει την τιμή **True**.</span><span class="sxs-lookup"><span data-stu-id="172c5-109">Run the PowerShell command [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) and verify that **AllowGiphy** is set to **TRUE**.</span></span>
- <span data-ttu-id="172c5-110">Εάν το **AllowGiphy** έχει καθοριστεί σε **False** , εκτελέστε την ακόλουθη εντολή PowerShell- [CsTeamsMessagingPolicy-ταυτότητα global-AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span><span class="sxs-lookup"><span data-stu-id="172c5-110">If **AllowGiphy** is set to **FALSE** , run the following PowerShell command [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span></span>

<span data-ttu-id="172c5-111">Οι [προαιρετικές συνδεδεμένες εμπειρίες](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) πρέπει να είναι ενεργοποιημένες για να επιτρέπουν την πρόσβαση στη διεύθυνση URL του GIPHY.</span><span class="sxs-lookup"><span data-stu-id="172c5-111">[Optional Connected Experiences](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) need to be enabled to allow access to the Giphy URL.</span></span>

> [!NOTE]
> <span data-ttu-id="172c5-112">Εάν έχετε ρυθμίσει πολλές πολιτικές ανταλλαγής μηνυμάτων ομάδων για τον μισθωτή σας, μπορείτε να προσδιορίσετε την ταυτότητα της πολιτικής που έχει εκχωρηθεί στον χρήστη με την εντολή PowerShell [Get-CsOnlineUser-Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Επιλέξτε TeamsMessagingPolicy.</span><span class="sxs-lookup"><span data-stu-id="172c5-112">If you have multiple Teams Messaging policies configured for your tenant, you can determine the identity of the policy assigned to the impacted user with the PowerShell command [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Select TeamsMessagingPolicy.</span></span>
