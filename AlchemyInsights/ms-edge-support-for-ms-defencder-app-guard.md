---
title: Υποστήριξη του Microsoft Edge για το προστατευτικό εφαρμογής του Microsoft Defender
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583584"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a><span data-ttu-id="3a696-102">Υποστήριξη του Microsoft Edge για το προστατευτικό εφαρμογής του Microsoft Defender</span><span class="sxs-lookup"><span data-stu-id="3a696-102">Microsoft Edge's support for Microsoft Defender Application Guard</span></span>

<span data-ttu-id="3a696-103">Σχεδιασμένο για Windows 10 και Microsoft Edge, το Guard εφαρμογών χρησιμοποιεί μια προσέγγιση απομόνωσης υλικού, η οποία επιτρέπει στους χρήστες να περιηγηθούν σε μη αξιόπιστες τοποθεσίες μέσα σε ένα απομονωμένο κοντέινερ με δυνατότητα Hyper-V, το οποίο διαχωρίζεται από το λειτουργικό σύστημα του κεντρικού υπολογιστή.</span><span class="sxs-lookup"><span data-stu-id="3a696-103">Designed for Windows 10 and Microsoft Edge, Application Guard uses a hardware-isolation approach that lets a user navigate an untrusted site from inside an isolated, Hyper-V–enabled container, separated from the host operating system.</span></span>

<span data-ttu-id="3a696-104">Ένας διαχειριστής εταιρείας ορίζει μια λίστα αξιόπιστων τοποθεσιών Web, πόρων cloud και εσωτερικών δικτύων.</span><span class="sxs-lookup"><span data-stu-id="3a696-104">An enterprise admin defines a list of trusted websites, cloud resources, and internal networks.</span></span> <span data-ttu-id="3a696-105">Όταν ένας χρήστης επισκέπτεται μια τοποθεσία που δεν υπάρχει στη λίστα, το Microsoft Edge θα ανοίξει την τοποθεσία στο κοντέινερ.</span><span class="sxs-lookup"><span data-stu-id="3a696-105">When a user visits a site that's not on the list, Microsoft Edge will open the site in the container.</span></span> <span data-ttu-id="3a696-106">Αυτό σημαίνει ότι εάν η τοποθεσία αποδειχθεί κακόβουλη, ο κεντρικός ΥΠΟΛΟΓΙΣΤΉς θα παραμείνει προστατευμένος και ο εισβολέας δεν θα φτάσει στα εταιρικά δεδομένα.</span><span class="sxs-lookup"><span data-stu-id="3a696-106">This means that if the site turns out to be malicious, the host PC will remain protected and the attacker won't get to the enterprise data.</span></span>

<span data-ttu-id="3a696-107">Η εγκατάσταση των επεκτάσεων στο κοντέινερ υποστηρίζεται από το Microsoft Edge έκδοση 81 και μπορεί να ελεγχθεί μέσω μιας πολιτικής.</span><span class="sxs-lookup"><span data-stu-id="3a696-107">Installation of extensions in the container is supported as of Microsoft Edge version 81, and it can be controlled via a policy.</span></span> <span data-ttu-id="3a696-108">Η διεύθυνση updateURL που χρησιμοποιείται στην πολιτική ExtensionInstallForcelist θα πρέπει να προστεθεί ως ουδέτερος πόρος στις πολιτικές απομόνωσης δικτύου που χρησιμοποιούνται από το Guard εφαρμογών.</span><span class="sxs-lookup"><span data-stu-id="3a696-108">The updateURL address that gets used in the ExtensionInstallForcelist policy should be added as a Neutral Resource in the Network Isolation policies used by Application Guard.</span></span>

<span data-ttu-id="3a696-109">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [υποστήριξη του Microsoft Edge για το προστατευτικό εφαρμογής του Microsoft Defender](https://go.microsoft.com/fwlink/?linkid=2134229).</span><span class="sxs-lookup"><span data-stu-id="3a696-109">For more info, see [Microsoft Edge support for Microsoft Defender Application Guard](https://go.microsoft.com/fwlink/?linkid=2134229).</span></span>