---
title: Ανάπτυξη του Microsoft Edge σε iOS, iPadOS και Android
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8241"
- "9004604"
ms.openlocfilehash: 524e87ab57e29823361053093708c83831f19687
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 02/10/2021
ms.locfileid: "50194523"
---
# <a name="deploy-microsoft-edge-to-ios-ipados-and-android"></a><span data-ttu-id="9596c-102">Ανάπτυξη του Microsoft Edge σε iOS, iPadOS και Android</span><span class="sxs-lookup"><span data-stu-id="9596c-102">Deploy Microsoft Edge to iOS, iPadOS, and Android</span></span>

<span data-ttu-id="9596c-103">Το καθοδηγούμενο σενάριο που συνοψίζεται παρακάτω θα σας βοηθήσει να εκχωρήσετε τον Microsoft Edge σε χρήστες συσκευών iOS, iPadOS και Android.</span><span class="sxs-lookup"><span data-stu-id="9596c-103">The guided scenario summarized below will help you assign Microsoft Edge to users of iOS, iPadOS, and Android devices.</span></span>

> [!NOTE]
> <span data-ttu-id="9596c-104">Εάν έχετε αποκλείσει χρήστες από την εγγραφή κινητών συσκευών, αυτό το καθοδηγούμενο σενάριο δεν θα λειτουργεί και οι χρήστες θα πρέπει να εγκαταστήσουν τον Microsoft Edge μόνοι τους.</span><span class="sxs-lookup"><span data-stu-id="9596c-104">If you blocked users from enrolling mobile devices, this guided scenario won't work and the users will need to install Microsoft Edge on their own.</span></span>

<span data-ttu-id="9596c-105">Το καθοδηγούμενο σενάριο περιλαμβάνει τα ακόλουθα βήματα:</span><span class="sxs-lookup"><span data-stu-id="9596c-105">The guided scenario involves the following steps:</span></span>

1. [<span data-ttu-id="9596c-106">Προαπαιτούμενα</span><span class="sxs-lookup"><span data-stu-id="9596c-106">Prerequisites</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#prerequisites)
2. [<span data-ttu-id="9596c-107">Εισαγωγή</span><span class="sxs-lookup"><span data-stu-id="9596c-107">Introduction</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-1---introduction)
3. [<span data-ttu-id="9596c-108">Βασικά στοιχεία</span><span class="sxs-lookup"><span data-stu-id="9596c-108">Basics</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-2---basics)
4. [<span data-ttu-id="9596c-109">Ρύθμιση παραμέτρων</span><span class="sxs-lookup"><span data-stu-id="9596c-109">Configuration</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-3---configuration)
5. [<span data-ttu-id="9596c-110">Αναθέσεις εργασιών</span><span class="sxs-lookup"><span data-stu-id="9596c-110">Assignments</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-4---assignments)
6. [<span data-ttu-id="9596c-111">Αναθεώρηση και δημιουργία</span><span class="sxs-lookup"><span data-stu-id="9596c-111">Review and creation</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-5---review--create)

<span data-ttu-id="9596c-112">Αφού ολοκληρώσετε τα βήματα στο καθοδηγούμενο σενάριο, οι πολιτικές του Microsoft Intune θα ενεργοποιήσουν τις ακόλουθες δυνατότητες του Microsoft Edge για επιχειρήσεις:</span><span class="sxs-lookup"><span data-stu-id="9596c-112">After you complete the steps in the guided scenario, Microsoft Intune policies will enable the following features of Microsoft Edge for business:</span></span>

- <span data-ttu-id="9596c-113">Διπλή ταυτότητα</span><span class="sxs-lookup"><span data-stu-id="9596c-113">Dual identity</span></span>
- <span data-ttu-id="9596c-114">Ενοποίηση με την πολιτική προστασίας εφαρμογών Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="9596c-114">Integration with Microsoft Intune app protection policy</span></span>
- <span data-ttu-id="9596c-115">Ενοποίηση με το διακομιστή μεσολάβησης εφαρμογών του Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="9596c-115">Integration with Azure Active Directory Application Proxy</span></span>
- <span data-ttu-id="9596c-116">Διαχειριζόμενα αγαπημένα και συντομεύσεις αρχικής σελίδας</span><span class="sxs-lookup"><span data-stu-id="9596c-116">Managed favorites and home page shortcuts</span></span>
