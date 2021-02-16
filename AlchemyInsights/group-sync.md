---
title: Συγχρονισμός ομάδας
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8304"
- "9003234"
ms.openlocfilehash: 52c19b6dcc79968150a188b389c5481c122f7945
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256717"
---
# <a name="group-sync"></a><span data-ttu-id="f5af3-102">Συγχρονισμός ομάδας</span><span class="sxs-lookup"><span data-stu-id="f5af3-102">Group sync</span></span>

<span data-ttu-id="f5af3-103">Αυτό το άρθρο παρέχει οδηγίες σχετικά με το συγχρονισμό ομάδων.</span><span class="sxs-lookup"><span data-stu-id="f5af3-103">This article provides guidance on group synchronization.</span></span>

1. <span data-ttu-id="f5af3-104">Εάν ένας καθολικός διαχειριστής ή κάτοχος ομάδας δεν μπορεί να τροποποιήσει τις ιδιότητες της ομάδας ή να προσθέσει μέλη ή να εκχωρήσει κατόχους στην πύλη Azure, βεβαιωθείτε ότι η προέλευση της αρχής για την ομάδα είναι το Azure Active Directory (Azure AD) για τον καθολικό διαχειριστή ή τον κάτοχο της ομάδας για να τροποποιήσει την ομάδα.</span><span class="sxs-lookup"><span data-stu-id="f5af3-104">If a global admin or group owner is not able to modify group properties or add members or assign owners in the Azure portal, ensure the source of the authority for the group is Azure Active Directory (Azure AD) for the global admin or group owner to modify the group.</span></span>
2. <span data-ttu-id="f5af3-105">Πριν προσπαθήσετε να διαγράψετε μια συγχρονισμένη ομάδα στο Azure AD, βεβαιωθείτε ότι έχετε διαγράψει όλες τις άδειες χρήσης που [έχουν εκχωρηθεί για](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced) να αποφύγετε τα σφάλματα.</span><span class="sxs-lookup"><span data-stu-id="f5af3-105">Before attempting to delete a synced group in Azure AD, ensure you have [deleted all assigned licenses](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced) to avoid errors.</span></span>

<span data-ttu-id="f5af3-106">Για να κατανοήσετε τον τρόπο με τον οποίο μπορείτε να συγχρονίσετε χρήστες, ομάδες και επαφές, ανατρέξτε στο θέμα "Συγχρονισμός [Azure AD Connect"](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts)και ακολουθήστε τον συγχρονισμό μιας ομάδας εσωτερικής εγκατάστασης στο Azure χρησιμοποιώντας το [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) για τον συγχρονισμό ομάδων εσωτερικής εγκατάστασης χρησιμοποιώντας το AD Connect.</span><span class="sxs-lookup"><span data-stu-id="f5af3-106">For understanding how to sync users, groups and contacts, see [Azure AD Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts), and follow [Syncing an on-premises group to Azure using Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) to sync on-perm groups using AD connect.</span></span>

<span data-ttu-id="f5af3-107">Ακολουθήστε αυτόν τον οδηγό [αντιμετώπισης σφαλμάτων κατά το συγχρονισμό για την](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) αντιμετώπιση συνηθισμένων σφαλμάτων κατά τη διάρκεια του συγχρονισμού.</span><span class="sxs-lookup"><span data-stu-id="f5af3-107">Follow this guide [Troubleshooting Errors during synchronization](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) to troubleshoot common errors during synchronization.</span></span>

