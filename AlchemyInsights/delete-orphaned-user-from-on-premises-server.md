---
title: Διαγραφή ορφανού χρήστη από διακομιστή εσωτερικής εγκατάστασης
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 7927c0684d2f5289f92506d7d05d5b1a3b43b658
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 07/20/2020
ms.locfileid: "45198186"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a><span data-ttu-id="9237e-102">Διαγραφή ορφανού χρήστη από διακομιστή εσωτερικής εγκατάστασης</span><span class="sxs-lookup"><span data-stu-id="9237e-102">Delete orphaned user from on-premises server</span></span>

<span data-ttu-id="9237e-103">Για να καταργήσετε έναν ορφανό χρήστη, ακολουθήστε τα εξής βήματα:</span><span class="sxs-lookup"><span data-stu-id="9237e-103">To remove an orphaned user, follow these steps:</span></span>

1. <span data-ttu-id="9237e-104">Επιβάλλετε το συγχρονισμό καταλόγου ακολουθώντας τις οδηγίες στην επιλογή [Τι είναι η υβριδική ταυτότητα με την υπηρεσία καταλόγου Azure Active Directory;](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span><span class="sxs-lookup"><span data-stu-id="9237e-104">Force directory synchronization by following the instructions in [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span></span>

2. <span data-ttu-id="9237e-105">Για να επαληθεύσετε το συγχρονισμό καταλόγου, ανατρέξτε στο θέμα [Τι είναι η υβριδική ταυτότητα με την υπηρεσία καταλόγου Azure Active Directory;](https://technet.microsoft.com/library/jj151797.aspx).</span><span class="sxs-lookup"><span data-stu-id="9237e-105">To verify directory synchronization, see [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span></span>

3. <span data-ttu-id="9237e-106">Εάν οι συναρτήσεις συγχρονισμού είναι σωστές, αλλά η διαγραφή αντικειμένου της υπηρεσίας καταλόγου Active Directory δεν μεταδίδεται στο Azure AD, καταργήστε με μη αυτόματο τρόπο το ορφανό αντικείμενο, χρησιμοποιώντας ένα από τα ακόλουθα cmdlet της λειτουργικής μονάδας azure active directory για windows PowerShell:</span><span class="sxs-lookup"><span data-stu-id="9237e-106">If sync functions correctly but the Active Directory object deletion does not propagate to Azure AD, manually remove the orphaned object by using one of the following Azure Active Directory Module for Windows PowerShell cmdlets:</span></span>

    <span data-ttu-id="9237e-107">Κατάργηση-MsolΕπικοίνετε</span><span class="sxs-lookup"><span data-stu-id="9237e-107">Remove-MsolContact</span></span>  
    <span data-ttu-id="9237e-108">Κατάργηση-MsolGroup</span><span class="sxs-lookup"><span data-stu-id="9237e-108">Remove-MsolGroup</span></span>  
    <span data-ttu-id="9237e-109">Κατάργηση χρήστη-msol</span><span class="sxs-lookup"><span data-stu-id="9237e-109">Remove-MsolUser</span></span>

    <span data-ttu-id="9237e-110">Για παράδειγμα, για να καταργήσετε ορφανά john.smith@contoso.com αναγνωριστικού χρήστη, το οποίο δημιουργήθηκε αρχικά χρησιμοποιώντας συγχρονισμό καταλόγου, εκτελέστε το cmdlet:</span><span class="sxs-lookup"><span data-stu-id="9237e-110">For example, to remove orphaned user ID john.smith@contoso.com, originally created by using directory synchronization, run the cmdlet:</span></span>

    <span data-ttu-id="9237e-111">Κατάργηση-MsolUser –UserPrincipalName John.Smith@Contoso.com</span><span class="sxs-lookup"><span data-stu-id="9237e-111">Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com</span></span>