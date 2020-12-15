---
title: Ανάπτυξη του Microsoft Edge για κινητές συσκευές για iOS/iPadOS ή Android
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
- "9003919"
- "6974"
ms.openlocfilehash: 98ab637b6ca0f2b3cfa98ae897d6ed1d9f36c3cd
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49678451"
---
# <a name="deploy-microsoft-edge-for-mobile-for-iosipados-or-android"></a><span data-ttu-id="06c04-102">Ανάπτυξη του Microsoft Edge για κινητές συσκευές για iOS/iPadOS ή Android</span><span class="sxs-lookup"><span data-stu-id="06c04-102">Deploy Microsoft Edge for Mobile for iOS/iPadOS or Android</span></span>

<span data-ttu-id="06c04-103">Το σενάριο με οδηγίες που συνοψίζεται παρακάτω θα σας βοηθήσει να αντιστοιχίσετε το Microsoft Edge σε χρήστες συσκευών iOS, iPadOS και Android.</span><span class="sxs-lookup"><span data-stu-id="06c04-103">The guided scenario summarized below will help you assign Microsoft Edge to users of iOS, iPadOS, and Android devices.</span></span> <span data-ttu-id="06c04-104">Αφού ολοκληρώσετε αυτά τα βήματα, οι πολιτικές του Microsoft Intune θα ενεργοποιήσουν τις ακόλουθες δυνατότητες του Microsoft Edge για επιχείρηση:</span><span class="sxs-lookup"><span data-stu-id="06c04-104">After you complete these steps, Microsoft Intune policies will enable the following features of Microsoft Edge for business:</span></span>

- <span data-ttu-id="06c04-105">Διπλή ταυτότητα</span><span class="sxs-lookup"><span data-stu-id="06c04-105">Dual identity</span></span>
- <span data-ttu-id="06c04-106">Ενοποίηση με την πολιτική προστασίας εφαρμογών του Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="06c04-106">Integration with Microsoft Intune app protection policy</span></span>
- <span data-ttu-id="06c04-107">Ενοποίηση με το διακομιστή μεσολάβησης εφαρμογής Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="06c04-107">Integration with Azure Active Directory Application Proxy</span></span>
- <span data-ttu-id="06c04-108">Διαχειριζόμενες συντομεύσεις αγαπημένων και αρχικών σελίδων</span><span class="sxs-lookup"><span data-stu-id="06c04-108">Managed favorites and home page shortcuts</span></span>

> [!NOTE]
> <span data-ttu-id="06c04-109">Εάν εμποδίσατε τους χρήστες να εγγραφούν σε κινητές συσκευές, αυτό το σενάριο καθοδηγούμενη δεν θα λειτουργήσει και οι χρήστες θα πρέπει να εγκαταστήσουν το Microsoft Edge μόνοι τους.</span><span class="sxs-lookup"><span data-stu-id="06c04-109">If you blocked users from enrolling mobile devices, this guided scenario will not work and the users will need to install Microsoft Edge on their own.</span></span>

<span data-ttu-id="06c04-110">Για να αναπτύξετε το Microsoft Edge για κινητές συσκευές για iOS/iPadOS ή Android, ανατρέξτε στα θέματα:</span><span class="sxs-lookup"><span data-stu-id="06c04-110">To deploy Microsoft Edge for Mobile for iOS/iPadOS or Android, see:</span></span>

1. [<span data-ttu-id="06c04-111">Τις προϋποθέσεις</span><span class="sxs-lookup"><span data-stu-id="06c04-111">Prerequisites</span></span>](https://go.microsoft.com/fwlink/?linkid=2133027)
2. [<span data-ttu-id="06c04-112">Εισαγωγή</span><span class="sxs-lookup"><span data-stu-id="06c04-112">Introduction</span></span>](https://go.microsoft.com/fwlink/?linkid=2133520)
3. [<span data-ttu-id="06c04-113">Βασικά στοιχεία</span><span class="sxs-lookup"><span data-stu-id="06c04-113">Basics</span></span>](https://go.microsoft.com/fwlink/?linkid=2133421)
4. [<span data-ttu-id="06c04-114">Παραμέτρων</span><span class="sxs-lookup"><span data-stu-id="06c04-114">Configuration</span></span>](https://go.microsoft.com/fwlink/?linkid=2133521)
5. [<span data-ttu-id="06c04-115">Αναθέσεις</span><span class="sxs-lookup"><span data-stu-id="06c04-115">Assignments</span></span>](https://go.microsoft.com/fwlink/?linkid=2132869)
6. [<span data-ttu-id="06c04-116">Αναθεώρηση και δημιουργία</span><span class="sxs-lookup"><span data-stu-id="06c04-116">Review and creation</span></span>](https://go.microsoft.com/fwlink/?linkid=2133522)
