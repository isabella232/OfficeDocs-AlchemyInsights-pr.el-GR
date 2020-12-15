---
title: Πώς να ενεργοποιήσετε το φιλοξενούμενο φωνητικό ταχυδρομείο
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7563"
ms.openlocfilehash: 26eb22054d246a6ca5a2491c68a5d9e4ed90d45b
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 12/09/2020
ms.locfileid: "49678002"
---
# <a name="how-to-enable-hosted-voicemail"></a><span data-ttu-id="4d2ad-102">Πώς να ενεργοποιήσετε το φιλοξενούμενο φωνητικό ταχυδρομείο</span><span class="sxs-lookup"><span data-stu-id="4d2ad-102">How to enable Hosted Voicemail</span></span>

<span data-ttu-id="4d2ad-103">Για να ενεργοποιήσετε το φωνητικό ταχυδρομείο, το **HostedVoicemail** πρέπει να έχει $True.</span><span class="sxs-lookup"><span data-stu-id="4d2ad-103">To enable Voicemail, **HostedVoicemail** must be set to $true.</span></span>

<span data-ttu-id="4d2ad-104">Η ιδιότητα **HostedVoicemail** στο χρήστη που χρησιμοποιεί το Remote POWERSHELL (RPS).</span><span class="sxs-lookup"><span data-stu-id="4d2ad-104">The **HostedVoicemail** property on the user using Remote PowerShell (RPS).</span></span>

<span data-ttu-id="4d2ad-105">Για περισσότερες πληροφορίες σχετικά με τη σύνδεση στο RPS, ανατρέξτε στο θέμα [Επισκόπηση του Microsoft teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) για περισσότερες πληροφορίες σχετικά με τη σύνδεση στο RPS.</span><span class="sxs-lookup"><span data-stu-id="4d2ad-105">For more information on connecting to RPS, see [Microsoft Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) for more information on connecting to RPS.</span></span>

1. <span data-ttu-id="4d2ad-106">Ο διαχειριστής των ομάδων θα πρέπει να συνδεθεί στο απομακρυσμένο PowerShell για ομάδες.</span><span class="sxs-lookup"><span data-stu-id="4d2ad-106">The Teams Admin should be logged into Remote PowerShell for Teams.</span></span>
1. <span data-ttu-id="4d2ad-107">Από την ερώτηση PowerShell, ο διαχειριστής των ομάδων μπορεί να εκτελέσει το πρόγραμμα **csuser user@contoso.com-HostedVoiceMail $True** όπου το URI SIP είναι του εν λόγω χρήστη.</span><span class="sxs-lookup"><span data-stu-id="4d2ad-107">From PowerShell prompt the Teams Admin can run **set-csuser user@contoso.com -HostedVoiceMail $true** where the sip uri is of the user in question.</span></span>

> [!NOTE]
> <span data-ttu-id="4d2ad-108">Οι αλλαγές στις πολιτικές μπορεί να χρειαστούν έως και 24 ώρες για την αναπαραγωγή.</span><span class="sxs-lookup"><span data-stu-id="4d2ad-108">Changes to policies can take up to 24 hours to replicate.</span></span>