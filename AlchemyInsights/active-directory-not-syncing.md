---
title: Η υπηρεσία καταλόγου Active Directory δεν συγχρονίζεται
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3abad160ab28922685d235a1fa546105e31757fb
ms.sourcegitcommit: d87a6ac6ee77375d1d750100359b4dc7b2871691
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 02/25/2020
ms.locfileid: "42265196"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="06682-102">Η υπηρεσία καταλόγου Active Directory δεν συγχρονίζεται</span><span class="sxs-lookup"><span data-stu-id="06682-102">Active Directory not syncing</span></span>

<span data-ttu-id="06682-103">Εάν λαμβάνετε σφάλματα συγχρονισμού, όπως "χωρίς πρόσφατο συγχρονισμό" ή παρατηρήσετε την κατάσταση συγχρονισμού καταλόγου στην πύλη διαχείρισης του Office λέει, "τελευταία συγχρονισμός περισσότερο από 3 ημέρες πριν," μπορεί να είναι ότι AADConnect έχει εσφαλμένες ρυθμίσεις ή ανεπαρκής δικαιώματα για την εκτέλεση συγχρονισμού.</span><span class="sxs-lookup"><span data-stu-id="06682-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="06682-104">Η επανεγκατάσταση του AADConnect χρησιμοποιώντας τις γρήγορες ρυθμίσεις ενδέχεται να επιλύσει το ζήτημα γρήγορα:</span><span class="sxs-lookup"><span data-stu-id="06682-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="06682-105">[Κατεβάστε την τελευταία έκδοση του AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span><span class="sxs-lookup"><span data-stu-id="06682-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="06682-106">[Ακολουθήστε τις οδηγίες για τη γρήγορη εγκατάσταση](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="06682-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="06682-107">Για περισσότερες πληροφορίες σχετικά με τους λογαριασμούς υπηρεσίας AADConnect, ανατρέξτε στο θέμα [σύνδεση AD Azure: λογαριασμοί και δικαιώματα](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="06682-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
