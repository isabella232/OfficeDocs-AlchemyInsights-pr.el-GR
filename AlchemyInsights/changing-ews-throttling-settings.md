---
title: Αλλαγή ρυθμίσεων ελέγχου EWS
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000752"
- "5653"
- "5760"
ms.openlocfilehash: 4f0bea884153dc1ed8699ce12e0d017d18f5e57c
ms.sourcegitcommit: 53e5caab697ebfb434ccef3ef98b8f2bee579b41
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 02/02/2021
ms.locfileid: "50075897"
---
# <a name="changing-ews-throttling-settings"></a><span data-ttu-id="b9ce0-102">Αλλαγή ρυθμίσεων ελέγχου EWS</span><span class="sxs-lookup"><span data-stu-id="b9ce0-102">Changing EWS throttling settings</span></span>

<span data-ttu-id="b9ce0-103">Εκτελέστε τον αυτοματοποιημένο έλεγχο που θα σας επιτρέψει να τροποποιήσετε την πολιτική ελέγχου EWS κατά τη διάρκεια της μετεγκατάστασης.</span><span class="sxs-lookup"><span data-stu-id="b9ce0-103">Please run our automated test which will allow you to modify the EWS throttling policy for the duration of your migration.</span></span> <span data-ttu-id="b9ce0-104">Σημειώστε ότι ακόμη και αφού εκτελεστεί αυτή η διαδικασία, οι εισαγωγές EWS θα εξακολουθούν να περιορίζονται στα 150mb ανά 5 λεπτά ανά γραμματοκιβώτιο. Για να επιτύχετε υψηλότερη ταχύτητα μετάδοσης μετεγκατάστασης, κάντε μετεγκατάσταση περισσότερων χρηστών ταυτόχρονα.</span><span class="sxs-lookup"><span data-stu-id="b9ce0-104">Note that even after this is run, EWS imports will still be limited to 150mb per 5 minutes per mailbox; to achieve higher migration throughput speeds, please migrate more users concurrently.</span></span>

<span data-ttu-id="b9ce0-105">Έχετε υπόψη ότι οι αλλαγές της πολιτικής ελέγχου EWS δεν έχουν καμία επίδραση στους ακόλουθους τύπους μετεγκατάστασης (χρησιμοποιώντας τα εργαλεία της Microsoft): Υβριδική, Πλήρης μεταφορά/Σταδιακή (RPC/HTTP), IMAP, G Suite, Δημόσιος φάκελος ή Υπηρεσία εισαγωγής PST.</span><span class="sxs-lookup"><span data-stu-id="b9ce0-105">Please note that EWS throttling policy changes have no effect on the following migration types (using Microsoft tools): Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Public Folder or PST Import Service.</span></span>