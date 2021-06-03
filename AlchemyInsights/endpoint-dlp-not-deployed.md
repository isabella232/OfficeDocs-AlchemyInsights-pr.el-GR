---
title: Το τελικό σημείο DLP δεν έχει αναπτυχθεί στη συσκευή του χρήστη
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11470"
- "9000292"
ms.openlocfilehash: 948835f5468b480536c176bfdf3b4eefb76b3bdb
ms.sourcegitcommit: c32233a1b7e6f1b07913d25f90189a58a8de2560
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52731584"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a><span data-ttu-id="b7439-102">Το τελικό σημείο DLP δεν έχει αναπτυχθεί στη συσκευή του χρήστη</span><span class="sxs-lookup"><span data-stu-id="b7439-102">Endpoint DLP not deployed to user's device</span></span>

<span data-ttu-id="b7439-103">Εάν η ρύθμιση αποτροπής απώλειας δεδομένων τελικού σημείου (DLP) δεν έχει εφαρμοστεί στη συσκευή ενός χρήστη, επιβεβαιώστε ότι πληροίτε αυτές τις απαιτήσεις:</span><span class="sxs-lookup"><span data-stu-id="b7439-103">If the Endpoint data loss prevention (DLP) setting has not applied to a user's device, confirm you meet these requirements:</span></span>

- <span data-ttu-id="b7439-104">Windows 10 έκδοση x64 1809 ή νεότερη έκδοση είναι εγκατεστημένη στη συσκευή.</span><span class="sxs-lookup"><span data-stu-id="b7439-104">Windows 10 x64 build 1809 or later is installed on the device.</span></span>
- <span data-ttu-id="b7439-105">Έχει εγκατασταθεί η έκδοση 4.18.2009.7 ή νεότερη έκδοση προγράμματος-πελάτη προστασίας από λογισμικό κακόβουλης λειτουργίας.</span><span class="sxs-lookup"><span data-stu-id="b7439-105">Anti-malware client version 4.18.2009.7 or later is installed.</span></span>
- <span data-ttu-id="b7439-106">Η συσκευή είναι **μία από** τις εξής:</span><span class="sxs-lookup"><span data-stu-id="b7439-106">The device is **one** of these:</span></span>
    
    - <span data-ttu-id="b7439-107">Azure Active Directory (Azure AD) συνδεδεμένος</span><span class="sxs-lookup"><span data-stu-id="b7439-107">Azure Active Directory (Azure AD) joined</span></span>
    - <span data-ttu-id="b7439-108">Υβριδική σύνδεση azure AD</span><span class="sxs-lookup"><span data-stu-id="b7439-108">Hybrid Azure AD joined</span></span>
    - <span data-ttu-id="b7439-109">Καταχωρημένο AAD</span><span class="sxs-lookup"><span data-stu-id="b7439-109">AAD registered</span></span>

- <span data-ttu-id="b7439-110">Για να επιβάλετε ενέργειες πολιτικής, βεβαιωθείτε ότι το πρόγραμμα Chromium Microsoft Edge είναι εγκατεστημένο στη συσκευή τελικού σημείου.</span><span class="sxs-lookup"><span data-stu-id="b7439-110">To enforce policy actions, make sure Microsoft Chromium Edge browser is installed on the endpoint device.</span></span>

<span data-ttu-id="b7439-111">Για πρόσθετες απαιτήσεις για την ανάπτυξη του DLP τελικού σημείου, ανατρέξτε στο θέμα [Γρήγορα αποτελέσματα με την αποτροπή απώλειας δεδομένων τελικού σημείου.](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints)</span><span class="sxs-lookup"><span data-stu-id="b7439-111">For additional requirements for deploying Endpoint DLP, see [Get started with Endpoint data loss prevention](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints).</span></span>