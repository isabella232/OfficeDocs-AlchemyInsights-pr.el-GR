---
title: Χρήση της αποτροπής παρακολούθησης στον Microsoft Edge (Chromium)
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8328"
- "9004625"
ms.openlocfilehash: 09e9a7303063328cd7bd0a0fcbf9629a3b38ebb5
ms.sourcegitcommit: 430d247cb5dd5dc5d1f82d977456558dfd514277
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51420869"
---
# <a name="use-tracking-prevention-in-microsoft-edge-chromium"></a><span data-ttu-id="96bc8-102">Χρήση της αποτροπής παρακολούθησης στον Microsoft Edge (Chromium)</span><span class="sxs-lookup"><span data-stu-id="96bc8-102">Use tracking prevention in Microsoft Edge (Chromium)</span></span>

<span data-ttu-id="96bc8-103">Η αποτροπή παρακολούθησης στον Microsoft Edge περιορίζει τη δυνατότητα ενός προγράμματος παρακολούθησης να αποκτήσει πρόσβαση στον χώρο αποθήκευσης που βασίζεται σε πρόγραμμα περιήγησης και στο δίκτυο.</span><span class="sxs-lookup"><span data-stu-id="96bc8-103">Tracking prevention in Microsoft Edge limits a tracker's ability to access browser-based storage and the network.</span></span> <span data-ttu-id="96bc8-104">Η δυνατότητα έχει δημιουργηθεί για να τηρεί τη δέσμευσή μας να βοηθά τους χρήστες να παραμένουν ασφαλείς στο web με τον Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="96bc8-104">The feature is built to uphold our commitment to helping users stay safe on the web with Microsoft Edge.</span></span> <span data-ttu-id="96bc8-105">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα Αποτροπή παρακολούθησης στον [Microsoft Edge (Chromium) και την](https://go.microsoft.com/fwlink/?linkid=2135435) υπόσχεσή μας για την προστασία [προσωπικών δεδομένων του προγράμματος περιήγησης .](https://go.microsoft.com/fwlink/?linkid=2135350)</span><span class="sxs-lookup"><span data-stu-id="96bc8-105">For more information, see [Tracking prevention in Microsoft Edge (Chromium)](https://go.microsoft.com/fwlink/?linkid=2135435) and [Our browser privacy promise](https://go.microsoft.com/fwlink/?linkid=2135350).</span></span>

<span data-ttu-id="96bc8-106">Ο Microsoft Edge προσφέρει τρία επίπεδα αποτροπής παρακολούθησης (μπορούν να επιλεγούν σε edge://settings/privacy):</span><span class="sxs-lookup"><span data-stu-id="96bc8-106">Microsoft Edge offers three levels of tracking prevention (they can be selected in edge://settings/privacy):</span></span>

- <span data-ttu-id="96bc8-107">**Το Βασικό** είναι το λιγότερο περιοριστικό και σχεδιασμένο για τους χρήστες που απολαμβάνουν εξατομικευμένες διαφημίσεις και δεν τους πειράζει να παρακολουθούνται στο web.</span><span class="sxs-lookup"><span data-stu-id="96bc8-107">**Basic** is the least restrictive and designed for users who enjoy personalized advertisements and don't mind being tracked on the web.</span></span> <span data-ttu-id="96bc8-108">Η "Βασική" προστατεύει τους χρήστες μόνο από κακόβουλα προγράμματα παρακολούθησης, όπως τα δακτυλικά αποτυπώματα και τα κρυπτονομίσματα.</span><span class="sxs-lookup"><span data-stu-id="96bc8-108">Basic protects users only against malicious trackers, such as fingerprinters and cryptominers.</span></span>
- <span data-ttu-id="96bc8-109">**Η εξισορρόπηση** είναι το προεπιλεγμένο επίπεδο και έχει σχεδιαστεί για τους χρήστες που θέλουν να βλέπουν λιγότερες διαφημίσεις που τους ακολουθούν στο web.</span><span class="sxs-lookup"><span data-stu-id="96bc8-109">**Balanced** is the default level and designed for users who want to see fewer advertisements that follow them around the web.</span></span> <span data-ttu-id="96bc8-110">Το ισορροπημένο επίπεδο έχει ως στόχο όχι μόνο τον αποκλεισμό των προγραμμάτων παρακολούθησης από τοποθεσίες με τις οποία οι χρήστες δεν συμμετέχουν ποτέ, αλλά και την ελαχιστοποίηση του κινδύνου προβλημάτων συμβατότητας.</span><span class="sxs-lookup"><span data-stu-id="96bc8-110">Balanced level aims not only to block trackers from sites that users never engage with but also to minimize the risk of compatibility issues.</span></span>
- <span data-ttu-id="96bc8-111">**Το strict** είναι το πιο περιοριστικό και σχεδιασμένο για τους χρήστες που δεν έχουν πρόβλημα να θυσιάσουν τη συμβατότητα των τοποθεσιών Web για μέγιστη προστασία προσωπικών δεδομένων.</span><span class="sxs-lookup"><span data-stu-id="96bc8-111">**Strict** is the most restrictive and designed for users who don't mind sacrificing website compatibility for maximum privacy.</span></span>