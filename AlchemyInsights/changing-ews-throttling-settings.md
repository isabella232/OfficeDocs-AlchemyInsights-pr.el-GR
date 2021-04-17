---
title: Αλλαγή ρυθμίσεων ελέγχου EWS
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 16916d5f16f763d87ce0d5ef830e741279c9f4df
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818036"
---
# <a name="changing-ews-throttling-settings"></a><span data-ttu-id="65023-102">Αλλαγή ρυθμίσεων ελέγχου EWS</span><span class="sxs-lookup"><span data-stu-id="65023-102">Changing EWS throttling settings</span></span>

<span data-ttu-id="65023-103">Εκτελέστε τον αυτοματοποιημένο έλεγχο που θα σας επιτρέψει να τροποποιήσετε την πολιτική ελέγχου EWS κατά τη διάρκεια της μετεγκατάστασης.</span><span class="sxs-lookup"><span data-stu-id="65023-103">Please run our automated test which will allow you to modify the EWS throttling policy for the duration of your migration.</span></span> <span data-ttu-id="65023-104">Σημειώστε ότι ακόμη και αφού εκτελεστεί αυτή η διαδικασία, οι εισαγωγές EWS θα εξακολουθούν να περιορίζονται στα 150mb ανά 5 λεπτά ανά γραμματοκιβώτιο. Για να επιτύχετε υψηλότερη ταχύτητα μετάδοσης μετεγκατάστασης, κάντε μετεγκατάσταση περισσότερων χρηστών ταυτόχρονα.</span><span class="sxs-lookup"><span data-stu-id="65023-104">Note that even after this is run, EWS imports will still be limited to 150mb per 5 minutes per mailbox; to achieve higher migration throughput speeds, please migrate more users concurrently.</span></span>

<span data-ttu-id="65023-105">Έχετε υπόψη ότι οι αλλαγές της πολιτικής ελέγχου EWS δεν έχουν καμία επίδραση στους ακόλουθους τύπους μετεγκατάστασης (χρησιμοποιώντας τα εργαλεία της Microsoft): Υβριδική, Πλήρης μεταφορά/Σταδιακή (RPC/HTTP), IMAP, G Suite, Δημόσιος φάκελος ή Υπηρεσία εισαγωγής PST.</span><span class="sxs-lookup"><span data-stu-id="65023-105">Please note that EWS throttling policy changes have no effect on the following migration types (using Microsoft tools): Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Public Folder or PST Import Service.</span></span>