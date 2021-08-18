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
ms.openlocfilehash: 4042e042554f78febff2073fde6f14db72a6d4e0
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58318648"
---
# <a name="how-to-enable-hosted-voicemail"></a>Τρόπος ενεργοποίησης του Φιλοξενούμενου φωνητικού ταχυδρομείου

Για να ενεργοποιήσετε το φωνητικό **ταχυδρομείο, το HostedVoicemail** πρέπει να έχει οριστεί σε $true.

Η **ιδιότητα HostedVoicemail** στο χρήστη που χρησιμοποιεί το Απομακρυσμένο PowerShell (RPS).

Για περισσότερες πληροφορίες σχετικά με τη σύνδεση στο RPS, ανατρέξτε [Microsoft Teams Επισκόπηση του PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) για περισσότερες πληροφορίες σχετικά με τη σύνδεση στο RPS.

1. Ο Teams διαχειριστής θα πρέπει να είναι συνδεδεμένος στο Απομακρυσμένο PowerShell για Teams.
1. Από το PowerShell, ο διαχειριστής του Teams μπορεί να εκτελέσει το **set-csuser user@contoso.com -HostedVoiceMail $true** όπου το sip uri είναι του εν λόγω χρήστη.

**Σημείωση:** Οι αλλαγές στις πολιτικές μπορεί να διαρκέσει έως και 24 ώρες για την αναπαραγωγή.