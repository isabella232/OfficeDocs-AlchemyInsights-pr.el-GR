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
# <a name="11-call-recording"></a><span data-ttu-id="a29b0-102">Εγγραφή κλήσης 1:1</span><span class="sxs-lookup"><span data-stu-id="a29b0-102">1:1 call recording</span></span>

<span data-ttu-id="a29b0-103">Οι διαχειριστές πρέπει να λάβουν μέτρα τώρα για να συνεχίσουν να επιτρέπουν στους χρήστες την εγγραφή κλήσεων 1:1.</span><span class="sxs-lookup"><span data-stu-id="a29b0-103">Administrators need to take action now to continue allowing users to Record 1:1 calls.</span></span>
 
<span data-ttu-id="a29b0-104">Από τις 12 Απριλίου 2021, θα ξεκινήσουμε την επιβολή μιας νέας επιλογής πολιτικής κλήσεων του Teams *AllowCloudRecordingForCalls.*</span><span class="sxs-lookup"><span data-stu-id="a29b0-104">Beginning April 12, 2021, we will start enforcing a new Teams Calling Policy option *AllowCloudRecordingForCalls*.</span></span> 

<span data-ttu-id="a29b0-105">Προς το παρόν, οι δυνατότητες εγγραφής κλήσεων 1:1 ελέγχονται από την *επιλογή AllowCloudRecording στις* Πολιτικές συσκέψεων του Teams.</span><span class="sxs-lookup"><span data-stu-id="a29b0-105">Currently 1:1 call recording capabilities are controlled by the *AllowCloudRecording* option in Teams Meeting Policies.</span></span> <span data-ttu-id="a29b0-106">Εάν οι χρήστες σας επιτρέπεται να καταγράφουν συσκέψεις του Teams, μπορούν επίσης να καταγράφουν 1:1 κλήσεις.</span><span class="sxs-lookup"><span data-stu-id="a29b0-106">If your users are allowed to record Teams Meetings they can also record 1:1 calls.</span></span>

<span data-ttu-id="a29b0-107">Εάν προτιμάτε να αποκλείσετε όλους τους χρήστες από την εγγραφή κλήσεων 1:1, δεν χρειάζεται να κάνετε καμία ενέργεια.</span><span class="sxs-lookup"><span data-stu-id="a29b0-107">If you prefer to block all users from recording 1:1 calls, you do not need to take any action.</span></span> <span data-ttu-id="a29b0-108">*Η επιλογή πολιτικής κλήσεων AllowCloudRecordingForCalls* θα $False από προεπιλογή.</span><span class="sxs-lookup"><span data-stu-id="a29b0-108">*AllowCloudRecordingForCalls* calling policy option will be $False by default.</span></span>

<span data-ttu-id="a29b0-109">Αυτή η αλλαγή τεκμηρρίζεται στην ακόλουθη δημοσίευση του Κέντρου μηνυμάτων: [(Ενημερώθηκε) 1:1](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) Εισαγωγή πολιτικής εγγραφής κλήσεων Για να ορίσετε την επιλογή πολιτικής κλήσεων του Teams, πρέπει να χρησιμοποιήσετε το [Teams PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-install)</span><span class="sxs-lookup"><span data-stu-id="a29b0-109">This change is documented in the following Message Center Post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) To set the Teams Calling Policy Option you must use [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install).</span></span>

<span data-ttu-id="a29b0-110">**Για να ενεργοποιήσετε την εγγραφή κλήσης σε κλήσεις 1:1:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True</span><span class="sxs-lookup"><span data-stu-id="a29b0-110">**To enable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True</span></span>

<span data-ttu-id="a29b0-111">**Για να απενεργοποιήσετε την εγγραφή κλήσης σε κλήσεις 1:1:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False</span><span class="sxs-lookup"><span data-stu-id="a29b0-111">**To disable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False</span></span>

