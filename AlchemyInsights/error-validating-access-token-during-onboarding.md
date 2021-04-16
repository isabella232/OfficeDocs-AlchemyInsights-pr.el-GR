---
title: Παρουσιάστηκε σφάλμα κατά την επικύρωση του διακριτικού πρόσβασης κατά την επιβιβα μένη ανάλυση επιφάνειας εργασίας
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 12e5906ba8cbc76ba1fd99dde1cf76396c3a6942
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813688"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="5b23f-102">Σφάλμα "Παρουσιάστηκε σφάλμα κατά την επικύρωση διακριτικού πρόσβασης" κατά την επιχείριση της Ανάλυσης επιφάνειας εργασίας</span><span class="sxs-lookup"><span data-stu-id="5b23f-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="5b23f-103">Αυτό το σφάλμα συνήθως παρατηρείται όταν λήξει το διακριτικό ελέγχου ταυτότητας.</span><span class="sxs-lookup"><span data-stu-id="5b23f-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="5b23f-104">Συνήθως, η ανανέωση της σελίδας ανανεώνει το διακριτικό.</span><span class="sxs-lookup"><span data-stu-id="5b23f-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="5b23f-105">Ωστόσο, αυτό το πρόβλημα μπορεί να συνεχιστεί εάν υπάρχουν πολιτικές πρόσβασης υπό όρους που εφαρμόζονται στο λογαριασμό που χρησιμοποιείται για την ανάλυση επιφάνειας εργασίας επί του πίνακα.</span><span class="sxs-lookup"><span data-stu-id="5b23f-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="5b23f-106">Μπορείτε να εξετάσετε τα αρχεία καταγραφής εισόδου του Azure AD στην Πύλη Azure για να δείτε εάν υπάρχουν αποτυχίες εισόδου για το λογαριασμό που χρησιμοποιείται για την εγγραφή στο Desktop Analytics.</span><span class="sxs-lookup"><span data-stu-id="5b23f-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="5b23f-107">Για περισσότερες πληροφορίες σχετικά με την πρόσβαση υπό όρους, επισκεφθείτε την [τοποθεσία "Σχεδιασμός ανάπτυξης πρόσβασης υπό όρους".](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)</span><span class="sxs-lookup"><span data-stu-id="5b23f-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>