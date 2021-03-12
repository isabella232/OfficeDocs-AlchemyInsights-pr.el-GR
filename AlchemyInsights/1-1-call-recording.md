---
title: Εγγραφή κλήσης 1:1
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "7648"
ms.openlocfilehash: af09e8805409446a42a62c82aa577ad27f09a17a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50733849"
---
# <a name="11-call-recording"></a>Εγγραφή κλήσης 1:1

Οι διαχειριστές πρέπει να λάβουν μέτρα τώρα για να συνεχίσουν να επιτρέπουν στους χρήστες την εγγραφή κλήσεων 1:1.
 
Από τις 12 Απριλίου 2021, θα ξεκινήσουμε την επιβολή μιας νέας επιλογής πολιτικής κλήσεων του Teams *AllowCloudRecordingForCalls.* 

Προς το παρόν, οι δυνατότητες εγγραφής κλήσεων 1:1 ελέγχονται από την *επιλογή AllowCloudRecording στις* Πολιτικές συσκέψεων του Teams. Εάν οι χρήστες σας επιτρέπεται να καταγράφουν συσκέψεις του Teams, μπορούν επίσης να καταγράφουν 1:1 κλήσεις.

Εάν προτιμάτε να αποκλείσετε όλους τους χρήστες από την εγγραφή κλήσεων 1:1, δεν χρειάζεται να κάνετε καμία ενέργεια. *Η επιλογή πολιτικής κλήσεων AllowCloudRecordingForCalls* θα $False από προεπιλογή.

Αυτή η αλλαγή τεκμηρρίζεται στην ακόλουθη δημοσίευση του Κέντρου μηνυμάτων: [(Ενημερώθηκε) 1:1](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) Εισαγωγή πολιτικής εγγραφής κλήσεων Για να ορίσετε την επιλογή πολιτικής κλήσεων του Teams, πρέπει να χρησιμοποιήσετε το [Teams PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-install)

**Για να ενεργοποιήσετε την εγγραφή κλήσης σε κλήσεις 1:1:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True

**Για να απενεργοποιήσετε την εγγραφή κλήσης σε κλήσεις 1:1:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False

