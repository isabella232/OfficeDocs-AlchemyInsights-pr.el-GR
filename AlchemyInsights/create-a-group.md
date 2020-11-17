---
title: Δημιουργία ομάδας
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
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088904"
---
# <a name="create-a-group"></a><span data-ttu-id="bb448-102">Δημιουργία ομάδας</span><span class="sxs-lookup"><span data-stu-id="bb448-102">Create a group</span></span>

<span data-ttu-id="bb448-103">Αυτό το θέμα περιγράφει τη δημιουργία ομάδας.</span><span class="sxs-lookup"><span data-stu-id="bb448-103">This topic describes group creation.</span></span>

<span data-ttu-id="bb448-104">**Δικαίωμα δημιουργίας ομάδας**</span><span class="sxs-lookup"><span data-stu-id="bb448-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="bb448-105">Βεβαιωθείτε ότι είστε εξουσιοδοτημένοι να δημιουργήσετε μια νέα ομάδα.</span><span class="sxs-lookup"><span data-stu-id="bb448-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="bb448-106">Οι Καθολικοί διαχειριστές μπορούν να απενεργοποιήσουν τη δημιουργία ομάδας στην πύλη Azure ή στον πίνακα πρόσβασης.</span><span class="sxs-lookup"><span data-stu-id="bb448-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="bb448-107">Μπορεί να χρειαστείτε ένα διαχειριστή για να δημιουργήσετε τη νέα ομάδα για εσάς ή για να σας παρέχει τα κατάλληλα δικαιώματα.</span><span class="sxs-lookup"><span data-stu-id="bb448-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="bb448-108">**Διαχείριση δικαιωμάτων δημιουργίας ομάδας**</span><span class="sxs-lookup"><span data-stu-id="bb448-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="bb448-109">Οι Καθολικοί διαχειριστές μπορούν να διαχειριστούν τα δικαιώματα δημιουργίας ομάδας (για λόγους που σχετίζονται με την ασφάλεια) ή τις ομάδες του Office 365 που δημιουργήθηκαν στην πύλη Azure ή στον πίνακα Access, επιλέγοντας "οι χρήστες μπορούν να δημιουργήσουν ομάδες ασφαλείας σε θύρες Azure" ή "οι χρήστες μπορούν να δημιουργήσουν ομάδες του Office 365 σε Azure portals" επιλογές σε όλες τις γενικές **ομάδες**  >  **(ρυθμίσεις)**.</span><span class="sxs-lookup"><span data-stu-id="bb448-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="bb448-110">Μπορείτε επίσης να περιορίσετε τη δημιουργία ομάδας για να επιλέξετε μια ομάδα χρηστών, εάν έχετε μια άδεια χρήσης του Azure Active Directory P1 Premium.</span><span class="sxs-lookup"><span data-stu-id="bb448-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="bb448-111">**Απενεργοποίηση ειδοποίησης καλωσορίσματος για τα νέα μέλη της ομάδας του Office 365**</span><span class="sxs-lookup"><span data-stu-id="bb448-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="bb448-112">Η ειδοποίηση καλωσορίσματος που στάλθηκε στους χρήστες που προστίθενται στο Office 365 Groups μπορεί να απενεργοποιηθεί ορίζοντας το **UnifiedGroupWelcomeMessageEnabled** σε FALSE στο PowerShell.</span><span class="sxs-lookup"><span data-stu-id="bb448-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="bb448-113">Μάθετε σχετικά με αυτήν τη ρύθμιση [εδώ](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="bb448-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

