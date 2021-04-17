---
title: Η υπηρεσία καταλόγου Active Directory δεν συγχρονίζεται
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
- "9001688"
- "3754"
ms.openlocfilehash: 274855457a143cfccd25f9a161ff894882cee9c4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822851"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="276f7-102">Η υπηρεσία καταλόγου Active Directory δεν συγχρονίζεται</span><span class="sxs-lookup"><span data-stu-id="276f7-102">Active Directory not syncing</span></span>

<span data-ttu-id="276f7-103">Εάν λαμβάνετε σφάλματα συγχρονισμού, όπως "δεν υπάρχει πρόσφατος συγχρονισμός" ή παρατηρήσετε ότι η κατάσταση συγχρονισμού καταλόγου στην πύλη διαχείρισης του Office αναφέρει "Ο τελευταίος συγχρονισμός έγινε πριν από περισσότερες από 3 ημέρες", μπορεί να είναι ότι το AADConnect έχει εσφαλμένες ρυθμίσεις ή ανεπαρκή δικαιώματα για την εκτέλεση συγχρονισμού.</span><span class="sxs-lookup"><span data-stu-id="276f7-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="276f7-104">Η επανεγκατάσταση του AADConnect με τη χρήση των express ρυθμίσεων μπορεί να επιλύσει το πρόβλημα γρήγορα:</span><span class="sxs-lookup"><span data-stu-id="276f7-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="276f7-105">[Κάντε λήψη της πιο πρόσφατης έκδοσης του AADConnect.](https://go.microsoft.com/fwlink/?LinkId=615771)</span><span class="sxs-lookup"><span data-stu-id="276f7-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="276f7-106">[Ακολουθήστε τις οδηγίες για τη γρήγορη εγκατάσταση.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)</span><span class="sxs-lookup"><span data-stu-id="276f7-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="276f7-107">Για περισσότερες πληροφορίες σχετικά με τους λογαριασμούς υπηρεσιών AADConnect, ανατρέξτε στο [θέμα Azure AD Connect: Λογαριασμοί και δικαιώματα.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)</span><span class="sxs-lookup"><span data-stu-id="276f7-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
