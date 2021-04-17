---
title: Δημιουργία ομάδας
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
- "9003234"
- "7230"
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816356"
---
# <a name="create-a-group"></a><span data-ttu-id="d33d6-102">Δημιουργία ομάδας</span><span class="sxs-lookup"><span data-stu-id="d33d6-102">Create a group</span></span>

<span data-ttu-id="d33d6-103">Αυτό το θέμα περιγράφει τη δημιουργία ομάδας.</span><span class="sxs-lookup"><span data-stu-id="d33d6-103">This topic describes group creation.</span></span>

<span data-ttu-id="d33d6-104">**Δικαίωμα δημιουργίας ομάδας**</span><span class="sxs-lookup"><span data-stu-id="d33d6-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="d33d6-105">Βεβαιωθείτε ότι έχετε την εξουσιοδότηση να δημιουργήσετε μια νέα ομάδα.</span><span class="sxs-lookup"><span data-stu-id="d33d6-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="d33d6-106">Οι καθολικοί διαχειριστές μπορούν να απενεργοποιήσουν τη δημιουργία ομάδας στην πύλη Azure ή στον Πίνακα πρόσβασης.</span><span class="sxs-lookup"><span data-stu-id="d33d6-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="d33d6-107">Μπορεί να χρειαστείτε ένα διαχειριστή για να δημιουργήσετε τη νέα ομάδα για εσάς ή για να σας δώσει τα κατάλληλα δικαιώματα.</span><span class="sxs-lookup"><span data-stu-id="d33d6-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="d33d6-108">**Διαχείριση δικαιωμάτων δημιουργίας ομάδας**</span><span class="sxs-lookup"><span data-stu-id="d33d6-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="d33d6-109">Οι καθολικοί διαχειριστές μπορούν να διαχειρίζονται δικαιώματα δημιουργίας ομάδων (για λόγους ασφαλείας) ή ομάδες του Office 365 που έχουν δημιουργηθεί στην πύλη Azure ή στον Πίνακα πρόσβασης, επιλέγοντας "Οι χρήστες μπορούν να δημιουργούν ομάδες ασφαλείας σε πύλες Azure" ή "Οι χρήστες μπορούν να δημιουργήσουν ομάδες του Office 365 σε πύλες Azure" στις επιλογές "Γενικά  >  **(Ρυθμίσεις)** όλων των ομάδων.</span><span class="sxs-lookup"><span data-stu-id="d33d6-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="d33d6-110">Μπορείτε επίσης να περιορίσετε τη δημιουργία ομάδας για να επιλέξετε μια ομάδα χρηστών, εάν έχετε μια άδεια χρήσης Azure Active Directory P1 Premium.</span><span class="sxs-lookup"><span data-stu-id="d33d6-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="d33d6-111">**Απενεργοποίηση ειδοποίησης υποδοχής για νέα μέλη ομάδας του Office 365**</span><span class="sxs-lookup"><span data-stu-id="d33d6-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="d33d6-112">Η ειδοποίηση υποδοχής που αποστέλλεται στους χρήστες που προστίθενται σε ομάδες του Office 365 μπορεί να απενεργοποιηθεί, ορίζοντας το **UnifiedGroupWelcomeMessageEnabled** σε False στο Powershell.</span><span class="sxs-lookup"><span data-stu-id="d33d6-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="d33d6-113">Μάθετε περισσότερα σχετικά με αυτήν τη [ρύθμιση εδώ.](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="d33d6-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

