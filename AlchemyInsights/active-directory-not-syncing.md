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
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: 0da512379e5a2f6ccb773e18c465e545c0660560
ms.sourcegitcommit: e42bb24c9bae1d0df8c49c424d2aa5e7466703ac
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/14/2021
ms.locfileid: "52930975"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="52b9a-102">Η υπηρεσία καταλόγου Active Directory δεν συγχρονίζεται</span><span class="sxs-lookup"><span data-stu-id="52b9a-102">Active Directory not syncing</span></span>

<span data-ttu-id="52b9a-103">Εάν λαμβάνετε σφάλματα συγχρονισμού, όπως "δεν υπάρχει πρόσφατος συγχρονισμός" ή παρατηρήσετε ότι η κατάσταση συγχρονισμού καταλόγου στην πύλη διαχείρισης του Office αναφέρει "Ο τελευταίος συγχρονισμός έγινε πριν από περισσότερες από 3 ημέρες", μπορεί να είναι ότι το AADConnect έχει εσφαλμένες ρυθμίσεις ή ανεπαρκή δικαιώματα για την εκτέλεση συγχρονισμού.</span><span class="sxs-lookup"><span data-stu-id="52b9a-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="52b9a-104">Η επανεγκατάσταση του AADConnect με χρήση των express ρυθμίσεων μπορεί να επιλύσει το πρόβλημα γρήγορα:</span><span class="sxs-lookup"><span data-stu-id="52b9a-104">Reinstalling AADConnect by using express settings might resolve the issue quickly:</span></span>

1. <span data-ttu-id="52b9a-105">[Κάντε λήψη της πιο πρόσφατης έκδοσης του AADConnect.](https://go.microsoft.com/fwlink/?LinkId=615771)</span><span class="sxs-lookup"><span data-stu-id="52b9a-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="52b9a-106">[Ακολουθήστε τις οδηγίες για τη γρήγορη εγκατάσταση.](/azure/active-directory/hybrid/how-to-connect-install-express)</span><span class="sxs-lookup"><span data-stu-id="52b9a-106">[Follow the instructions for express installation](/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="52b9a-107">Το Azure AD Connect πρέπει να είναι εγκατεστημένο στον Windows Server 2012 ή σε νεότερες εκδόσεις.</span><span class="sxs-lookup"><span data-stu-id="52b9a-107">Azure AD Connect must be installed on Windows Server 2012 or later.</span></span> <span data-ttu-id="52b9a-108">Αυτός ο διακομιστής πρέπει να είναι συνδεδεμένος με τομέα και μπορεί να είναι ελεγκτής τομέα ή διακομιστής-μέλος.</span><span class="sxs-lookup"><span data-stu-id="52b9a-108">This server must be domain joined and may be a domain controller or a member server.</span></span> <span data-ttu-id="52b9a-109">Για μια πλήρη λίστα με τις απαιτήσεις Σύνδεση Azure AD και τα προαπαιτούμενα, εξετάστε τις [προϋποθέσεις για το Azure AD Σύνδεση.](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)</span><span class="sxs-lookup"><span data-stu-id="52b9a-109">For a full list of Azure AD Connect requirements and pre-requisites, review [Prerequisites for Azure AD Connect](/azure/active-directory/hybrid/how-to-connect-install-prerequisites).</span></span>

<span data-ttu-id="52b9a-110">Για περισσότερες πληροφορίες σχετικά με τους λογαριασμούς υπηρεσιών AADConnect, ανατρέξτε στο [θέμα Azure AD Σύνδεση: Λογαριασμοί και δικαιώματα.](/azure/active-directory/hybrid/reference-connect-accounts-permissions)</span><span class="sxs-lookup"><span data-stu-id="52b9a-110">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
