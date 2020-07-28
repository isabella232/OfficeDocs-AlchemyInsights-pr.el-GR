---
title: Πολλαπλές ενεργές περιόδους λειτουργίας στο ίδιο γραμματοκιβώτιο
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1836"
- "9000248"
ms.openlocfilehash: d2fd3f20346012baed21efd4900ca4cf73391d91
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439196"
---
# <a name="multiple-active-sessions-to-the-same-mailbox"></a><span data-ttu-id="d37e2-102">Πολλαπλές ενεργές περιόδους λειτουργίας στο ίδιο γραμματοκιβώτιο</span><span class="sxs-lookup"><span data-stu-id="d37e2-102">Multiple active sessions to the same mailbox</span></span>

<span data-ttu-id="d37e2-103">Για να ελέγξετε τη χρήση των πόρων του Exchange, ένα γραμματοκιβώτιο έχει έναν "προϋπολογισμό".</span><span class="sxs-lookup"><span data-stu-id="d37e2-103">To control usage of Exchange resources, a mailbox has a "budget."</span></span>

<span data-ttu-id="d37e2-104">Η εξαίρεση που έχει υπεραποτολογηθεί μπορεί να προκληθεί από τις ακόλουθες περιπτώσεις, αλλά δεν περιορίζεται σε αυτές:</span><span class="sxs-lookup"><span data-stu-id="d37e2-104">The over-budget exception can be triggered by, but is not limited to, the following circumstances:</span></span>

- <span data-ttu-id="d37e2-105">Μερικές καρτέλες προγράμματος περιήγησης ανοίγουν στην ίδια περίοδο λειτουργίας του Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="d37e2-105">A few browser tabs are opened within the same Outlook Web App session.</span></span>

- <span data-ttu-id="d37e2-106">Μερικές ενεργές περιόδους λειτουργίας του Outlook Web App στο ίδιο γραμματοκιβώτιο.</span><span class="sxs-lookup"><span data-stu-id="d37e2-106">A few active Outlook Web App sessions to the same mailbox.</span></span>

- <span data-ttu-id="d37e2-107">Μερικές άλλες εφαρμογές-πελάτες (Outlook, Outlook Mobile, μια εφαρμογή προγράμματος-πελάτη άλλου κατασκευαστή) έχουν πρόσβαση στο γραμματοκιβώτιο ταυτόχρονα.</span><span class="sxs-lookup"><span data-stu-id="d37e2-107">A few other client applications (Outlook, Outlook Mobile, a third party client app) access the mailbox at the same time.</span></span>

- <span data-ttu-id="d37e2-108">Οι λειτουργίες μεγάλης διάρκειας, όπως η εκτέλεση αιτήσεων αναζήτησης, εκτελούνται από άλλη ενεργή περίοδο λειτουργίας γραμματοκιβωτίου.</span><span class="sxs-lookup"><span data-stu-id="d37e2-108">Long running operations, such as executing search requests, are performed from another active mailbox session.</span></span>

