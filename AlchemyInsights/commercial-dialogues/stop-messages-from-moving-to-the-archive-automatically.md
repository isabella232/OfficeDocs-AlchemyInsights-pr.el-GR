---
title: Διακοπή της αυτόματης μετακίνησης μηνυμάτων στην αρχειοθήκη
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 2cb3e29dfd4f422e946b7887d4d44f373ff03794
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746332"
---
# <a name="stop-messages-from-moving-to-the-archive-automatically"></a><span data-ttu-id="a5145-102">Διακοπή της αυτόματης μετακίνησης μηνυμάτων στην αρχειοθήκη</span><span class="sxs-lookup"><span data-stu-id="a5145-102">Stop messages from moving to the archive automatically</span></span>

<span data-ttu-id="a5145-103">Εάν χρησιμοποιείτε μια πολιτική διατήρησης, μπορείτε να αλλάξετε την ηλικία διατήρησης σε αυτή την πολιτική για να διακόψετε την αυτόματη αρχειοθέτηση των μηνυμάτων.</span><span class="sxs-lookup"><span data-stu-id="a5145-103">If you are using a retention policy, you can change the retention age in that policy to stop messages from archiving automatically.</span></span> <span data-ttu-id="a5145-104">Αυτό μπορεί να γίνει ως εξής:</span><span class="sxs-lookup"><span data-stu-id="a5145-104">Here's how:</span></span>

1. <span data-ttu-id="a5145-105">Στο κέντρο [διαχείρισης του Exchange, επιλέξτε](https://go.microsoft.com/fwlink/?linkid=2059104) **ετικέτες διατήρησης διαχείρισης**  >  **συμμόρφωσης.**</span><span class="sxs-lookup"><span data-stu-id="a5145-105">In the [Exchange admin center](https://go.microsoft.com/fwlink/?linkid=2059104), choose **compliance management** > **retention tags**.</span></span> <span data-ttu-id="a5145-106">Εντοπίστε την ετικέτα διατήρησης "Μετακίνηση σε αρχειοθέτηση".</span><span class="sxs-lookup"><span data-stu-id="a5145-106">Locate your Move to Archive retention tag.</span></span>
2. <span data-ttu-id="a5145-107">Στην ετικέτα διατήρησης, αλλάξτε την περίοδο διατήρησης (περίοδος αρχειοθέτησης) σε **"Ποτέ"** για να διακόψετε την αυτόματη αρχειοθέτηση των στοιχείων από μια πολιτική διατήρησης.</span><span class="sxs-lookup"><span data-stu-id="a5145-107">In the retention tag, change the retention period (archive period) to **Never** to stop items from being automatically archived by a retention policy.</span></span>

> [!NOTE]
> <span data-ttu-id="a5145-108">Αυτό θα αλλάξει τη ρύθμιση αρχειοθέτησης για όλα τα γραμματοκιβώτια στα οποία έχει εφαρμοστεί αυτή η ετικέτα διατήρησης.</span><span class="sxs-lookup"><span data-stu-id="a5145-108">This will change the archive setting for all mailboxes with this retention tag applied to them.</span></span>
