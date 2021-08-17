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
ms.openlocfilehash: c17408442cec6c0877b7d66bc8a7fd3062eb0e47
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314384"
---
# <a name="11-call-recording"></a>Εγγραφή κλήσης 1:1

Εάν το **κουμπί "Έναρξη** εγγραφής" είναι γκρι σε μια κλήση 1:1, πρέπει να αλλάξετε τις ρυθμίσεις πολιτικής για τον χρήστη που έχει επιπτώσεις. Για να ελέγξετε τη ρύθμιση πολιτικής, εκτελέστε το Διαγνωστικό για τον χρήστη που έχει επιπτώσεις πληκτρολογώντας **Diag: Teams 1:1 Εγγραφή κλήσης** παραπάνω.     

Από τις 31 Μαΐου 2021, θα ξεκινήσουμε την επιβολή μιας νέας πολιτικής κλήσεων Teams *AllowCloudRecordingForCalls.* Πριν από αυτή την αλλαγή, η εγγραφή κλήσης 1:1 ελέγχεται από την Πολιτική Teams *AllowCloudRecording.* Αυτή η αλλαγή τεκμηρροποιείται στη δημοσίευση του Κέντρου μηνυμάτων: [(Ενημερώθηκε) 1:1 Εισαγωγή πολιτικής εγγραφής κλήσεων.](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)  

*AllowCloudRecordingForCalls*   Η επιλογή πολιτικής κλήσεων έχει **οριστεί σε $False** από προεπιλογή. Εάν προτιμάτε να αποκλείσετε όλους τους χρήστες από την εγγραφή κλήσεων 1:1, δεν χρειάζεται να κάνετε καμία ενέργεια.  

Για να ενεργοποιήσετε την εγγραφή κλήσης για όλους τους χρήστες σε κλήσεις 1:1, [χρησιμοποιήστε Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install) για να εκτελέσετε το ακόλουθο cmdlet: 

**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True** 

Εναλλακτικά, μπορείτε να δημιουργήσετε μια νέα πολιτική και να ορίσετε **-AllowCloudRecordingForCalls** σε **$true και** να αντιστοιχίσετε αυτήν την πολιτική στους χρήστες σας. 

Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα 1:1 Τα στοιχεία ελέγχου πολιτικής εγγραφής κλήσεων είναι (σχεδόν!) Εδώ.](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668)
