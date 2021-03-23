---
title: Αντιμετώπιση προβλημάτων του κωδικού σφάλματος AADSTS650056
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9803"
- "9005744"
ms.openlocfilehash: 945be2b496b98937bfae6d1f573162d1f2ebb4b6
ms.sourcegitcommit: 1d73771d147325cfd8578e6816becd8331913890
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036649"
---
# <a name="troubleshoot-error-code-aadsts650056"></a><span data-ttu-id="69d2f-102">Αντιμετώπιση προβλημάτων του κωδικού σφάλματος AADSTS650056</span><span class="sxs-lookup"><span data-stu-id="69d2f-102">Troubleshoot error code AADSTS650056</span></span>

<span data-ttu-id="69d2f-103">Για να επιλύσετε το σφάλμα AADSTS650056, εκτελέστε το παρακάτω προτεινόμενο βήμα.</span><span class="sxs-lookup"><span data-stu-id="69d2f-103">To resolve AADSTS650056 error, perform the below recommended step.</span></span>

<span data-ttu-id="69d2f-104">**AADSTS65005:** MisconfiguredApplication - Η λίστα πρόσβασης πόρων που απαιτείται από την εφαρμογή δεν περιέχει εφαρμογές που είναι ανιχνεύσιμες από τον πόρο ή η εφαρμογή-πελάτης έχει ζητήσει πρόσβαση σε πόρο, η οποία δεν καθορίστηκε στην απαιτούμενη λίστα πρόσβασης πόρων ή η υπηρεσία Graph επέστρεψε εσφαλμένη αίτηση ή δεν βρέθηκε πόρος.</span><span class="sxs-lookup"><span data-stu-id="69d2f-104">**AADSTS65005**: MisconfiguredApplication - The app required resource access list does not contain apps discoverable by the resource or The client app has requested access to resource, which was not specified in its required resource access list or Graph service returned bad request or resource not found.</span></span> <span data-ttu-id="69d2f-105">Εάν η εφαρμογή υποστηρίζει SAML, ενδέχεται να έχετε ρυθμίσει τις παραμέτρους της εφαρμογής με λάθος αναγνωριστικό (Οντότητα).</span><span class="sxs-lookup"><span data-stu-id="69d2f-105">If the app supports SAML, you may have configured the app with the wrong Identifier (Entity).</span></span>

<span data-ttu-id="69d2f-106">Για περισσότερες πληροφορίες, ανατρέξτε στο άρθρο αντιμετώπισης προβλημάτων για το [σφάλμα AADSTS650056.](https://docs.microsoft.com/troubleshoot/azure/active-directory/error-code-aadsts650056-misconfigured-app)</span><span class="sxs-lookup"><span data-stu-id="69d2f-106">For more information, see the troubleshooting article for error [AADSTS650056](https://docs.microsoft.com/troubleshoot/azure/active-directory/error-code-aadsts650056-misconfigured-app).</span></span>
