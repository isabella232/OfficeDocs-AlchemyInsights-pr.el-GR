---
title: Τρόπος ενεργοποίησης του Φιλοξενούμενου φωνητικού ταχυδρομείου
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
ms.openlocfilehash: 4d70e92a7c1bf8f3cc62d4a310aa140ee2dfdef4c798ae17faa961736d9db500
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54055554"
---
# <a name="how-to-enable-hosted-voicemail"></a>Τρόπος ενεργοποίησης του Φιλοξενούμενου φωνητικού ταχυδρομείου

Για να ενεργοποιήσετε το Φωνητικό **ταχυδρομείο, το HostedVoicemail** πρέπει να έχει οριστεί σε $true.

Η **ιδιότητα HostedVoicemail** στο χρήστη που χρησιμοποιεί το Απομακρυσμένο PowerShell (RPS).

Για περισσότερες πληροφορίες σχετικά με τη σύνδεση στο RPS, ανατρέξτε Microsoft Teams επισκόπηση του [PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) για περισσότερες πληροφορίες σχετικά με τη σύνδεση στο RPS.

1. Ο Teams διαχειριστής θα πρέπει να συνδεθεί στο Απομακρυσμένο PowerShell για Teams.
1. Από το PowerShell, ο διαχειριστής του Teams μπορεί να εκτελέσει το **set-csuser user@contoso.com -HostedVoiceMail $true** όπου το sip uri είναι του εν λόγω χρήστη.

> [!NOTE]
> Οι αλλαγές στις πολιτικές μπορεί να διαρκέσει έως και 24 ώρες για την αναπαραγωγή.