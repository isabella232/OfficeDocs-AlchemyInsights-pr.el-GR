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
ms.openlocfilehash: 18c68fee514681b2a81c3cfa022c29ce83834f22
ms.sourcegitcommit: 610a5d950cdf488870601762ef52d881e3e22a48
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 05/28/2021
ms.locfileid: "52696923"
---
# <a name="11-call-recording"></a><span data-ttu-id="470f3-102">Εγγραφή κλήσης 1:1</span><span class="sxs-lookup"><span data-stu-id="470f3-102">1:1 call recording</span></span>

<span data-ttu-id="470f3-103">Εάν το **κουμπί "Έναρξη** εγγραφής" είναι γκρι σε μια κλήση 1:1, πρέπει να αλλάξετε τις ρυθμίσεις πολιτικής για τον χρήστη που έχει επιπτώσεις.</span><span class="sxs-lookup"><span data-stu-id="470f3-103">If the **Start Recording** button is grayed out in a 1:1 call, you need to change the policy settings for the impacted user.</span></span>   

<span data-ttu-id="470f3-104">Από τις 31 Μαΐου 2021, θα ξεκινήσουμε την επιβολή μιας νέας πολιτικής κλήσεων Teams *AllowCloudRecordingForCalls.*</span><span class="sxs-lookup"><span data-stu-id="470f3-104">Beginning May 31, 2021, we'll start enforcing a new Teams Calling Policy *AllowCloudRecordingForCalls*.</span></span> <span data-ttu-id="470f3-105">Πριν από αυτή την αλλαγή, η εγγραφή κλήσης 1:1 ελέγχεται από την Πολιτική Teams *AllowCloudRecording.*</span><span class="sxs-lookup"><span data-stu-id="470f3-105">Prior to this change, 1:1 call recording is controlled by the *AllowCloudRecording* Teams Meeting Policy.</span></span> <span data-ttu-id="470f3-106">Αυτή η αλλαγή τεκμηρροποιείται στη δημοσίευση του Κέντρου μηνυμάτων: [(Ενημερώθηκε) 1:1 Εισαγωγή πολιτικής εγγραφής κλήσεων.](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)</span><span class="sxs-lookup"><span data-stu-id="470f3-106">This change is documented in the Message Center post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).</span></span>  

<span data-ttu-id="470f3-107">*AllowCloudRecordingForCalls*   Η επιλογή πολιτικής κλήσεων έχει **οριστεί σε $False** από προεπιλογή.</span><span class="sxs-lookup"><span data-stu-id="470f3-107">*AllowCloudRecordingForCalls* calling policy option is set to **$False** by default.</span></span> <span data-ttu-id="470f3-108">Εάν προτιμάτε να αποκλείσετε όλους τους χρήστες από την εγγραφή κλήσεων 1:1, δεν χρειάζεται να κάνετε καμία ενέργεια.</span><span class="sxs-lookup"><span data-stu-id="470f3-108">If you prefer to block all users from recording 1:1 calls, you don't need to take any action.</span></span>  

<span data-ttu-id="470f3-109">Για να ενεργοποιήσετε την εγγραφή κλήσης για όλους τους χρήστες σε κλήσεις 1:1, χρησιμοποιήστε Teams PowerShell για να εκτελέσετε το ακόλουθο cmdlet:</span><span class="sxs-lookup"><span data-stu-id="470f3-109">To enable call recording for all users in 1:1 calls use Teams PowerShell to run the following cmdlet:</span></span> 

<span data-ttu-id="470f3-110">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span><span class="sxs-lookup"><span data-stu-id="470f3-110">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span></span> 

<span data-ttu-id="470f3-111">Εναλλακτικά, μπορείτε να δημιουργήσετε μια νέα πολιτική και να ορίσετε **-AllowCloudRecordingForCalls** σε **$true και** να εκχωρήσετε αυτήν την πολιτική στους χρήστες σας.</span><span class="sxs-lookup"><span data-stu-id="470f3-111">Alternatively, you can create a new policy and set **-AllowCloudRecordingForCalls** to **$true** and assign that policy to your users.</span></span> 

<span data-ttu-id="470f3-112">Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα 1:1 Τα στοιχεία ελέγχου πολιτικής εγγραφής κλήσεων είναι (σχεδόν!) Εδώ.](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668)</span><span class="sxs-lookup"><span data-stu-id="470f3-112">For more information, see [1:1 Call Recording Policy Controls Are (Almost!) Here](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span></span>
