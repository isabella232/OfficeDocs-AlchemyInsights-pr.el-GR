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
# <a name="how-to-enable-hosted-voicemail"></a>Πώς να ενεργοποιήσετε το φιλοξενούμενο φωνητικό ταχυδρομείο

Για να ενεργοποιήσετε το φωνητικό ταχυδρομείο, το **HostedVoicemail** πρέπει να έχει $True.

Η ιδιότητα **HostedVoicemail** στο χρήστη που χρησιμοποιεί το Remote POWERSHELL (RPS).

Για περισσότερες πληροφορίες σχετικά με τη σύνδεση στο RPS, ανατρέξτε στο θέμα [Επισκόπηση του Microsoft teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) για περισσότερες πληροφορίες σχετικά με τη σύνδεση στο RPS.

1. Ο διαχειριστής των ομάδων θα πρέπει να συνδεθεί στο απομακρυσμένο PowerShell για ομάδες.
1. Από την ερώτηση PowerShell, ο διαχειριστής των ομάδων μπορεί να εκτελέσει το πρόγραμμα **csuser user@contoso.com-HostedVoiceMail $True** όπου το URI SIP είναι του εν λόγω χρήστη.

> [!NOTE]
> Οι αλλαγές στις πολιτικές μπορεί να χρειαστούν έως και 24 ώρες για την αναπαραγωγή.