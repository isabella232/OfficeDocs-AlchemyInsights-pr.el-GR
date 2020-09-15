---
title: Ο συγχρονισμός της υπηρεσίας καταλόγου Active Directory δεν είναι
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3517f424b4dcd89f915acebab747a9bff993fdbd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47697629"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="d51c1-102">Ο συγχρονισμός της υπηρεσίας καταλόγου Active Directory δεν είναι</span><span class="sxs-lookup"><span data-stu-id="d51c1-102">Active Directory not syncing</span></span>

<span data-ttu-id="d51c1-103">Εάν λαμβάνετε σφάλματα συγχρονισμού, όπως "χωρίς πρόσφατο συγχρονισμό" ή Παρατηρήστε ότι η κατάσταση συγχρονισμού καταλόγου στην πύλη διαχείρισης του Office αναφέρει ότι "τελευταία συγχρονισμός πριν από περισσότερες από 3 ημέρες", μπορεί να είναι ότι το AADConnect έχει εσφαλμένες ρυθμίσεις ή ανεπαρκή δικαιώματα για την εκτέλεση συγχρονισμού.</span><span class="sxs-lookup"><span data-stu-id="d51c1-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="d51c1-104">Η επανεγκατάσταση του AADConnect με τη χρήση των ρυθμίσεων Express μπορεί να επιλύσει το πρόβλημα γρήγορα:</span><span class="sxs-lookup"><span data-stu-id="d51c1-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="d51c1-105">[Πραγματοποιήστε λήψη της τελευταίας έκδοσης του AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span><span class="sxs-lookup"><span data-stu-id="d51c1-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="d51c1-106">[Ακολουθήστε τις οδηγίες για τη γρήγορη εγκατάσταση](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="d51c1-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="d51c1-107">Για περισσότερες πληροφορίες σχετικά με τους λογαριασμούς υπηρεσίας AADConnect, ανατρέξτε στο θέμα [σύνδεση του Azure AD: λογαριασμοί και δικαιώματα](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="d51c1-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
